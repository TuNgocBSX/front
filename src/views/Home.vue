<template>
<div style="margin-left: 5%">
    <div>
        <b-card title="Xem tỷ lệ" tag="article" style="max-width: 20rem;" class="mb-2">
            <b-form inline>
                <b-input-group class="mb-2 mr-sm-2 mb-sm-0" prepend="Tổng số" style="margin-top:10px">
                    <b-input id="inline-form-input-name" class="mb-2 mr-sm-2 mb-sm-0" v-model="total" placeholder="40"></b-input>
                </b-input-group>

                <b-input-group class="mb-2 mr-sm-2 mb-sm-0" prepend="bắt đầu" style="margin-top:10px">
                    <b-input id="inline-form-input-username" v-model="start" placeholder="72800"></b-input>
                </b-input-group>

                <b-input-group class="mb-2 mr-sm-2 mb-sm-0" prepend="kết thúc" style="margin-top:10px">
                    <b-input id="inline-form-input-username" v-model="end" placeholder="72999"></b-input>
                </b-input-group>
                <b-input-group prepend="kết thúc" style="margin-top:10px" class="mb-2 mr-sm-2 mb-sm-0">
                    <b-input id="inline-form-input-username" v-model="num" placeholder="Số xem"></b-input>
                </b-input-group>
                <b-button variant="primary" style="margin-top:10px" @click="viewper">xem</b-button>
            </b-form>
        </b-card>
        <b-alert :show="isactive">{{ result }} %</b-alert>
    </div>
    <div style="margin-top: 10px">
        <b-card title="Nhập số mới" tag="article" style="max-width: 20rem;" class="mb-2">
            <b-form inline>
                <label class="sr-only" for="inline-form-input-username">Số mới</label>
                <b-input-group class="mb-2 mr-sm-2 mb-sm-0">
                    <b-input id="inline-form-input-username" v-model="number" placeholder="Số mới"></b-input>
                </b-input-group>
                <b-button variant="primary" @click="add">lưu</b-button>
            </b-form>
        </b-card>
    </div>
</div>
</template>

<script>
import axios from "../axios";
export default {
    data() {
        return {
            start: "",
            end: "",
            total: "",
            num: "",
            number: "",

            result: "",
            isactive: false,
        };
    },
    methods: {
        viewper() {
            const start = parseInt(this.start, 10);
            const end = parseInt(this.end, 10);
            const total = parseInt(this.total, 10);
            axios
                .post("/per", {
                    start,
                    end,
                    total,
                })
                .then((res) => {
                    this.isactive = true;
                    this.result = res.body;
                });
        },
        add() {
            const number = parseInt(this.number, 10);
            axios
                .post("/", {
                    num: number,
                })
                .then((res) => {
                    this.isactive = true;
                    this.result = res.body;
                });
        },
    },
};
</script>
