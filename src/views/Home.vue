<template>
<div style="width: 100%;height:100%">
    <e-charts :options="line" theme="ovilia-green" ref="line" />
    <p>p1</p>
    <e-charts :options="line2" theme="ovilia-green" ref="line" />
    <p>p2</p>
    <e-charts :options="line" theme="ovilia-green" ref="line" />
    <p>p1</p>
    <e-charts :options="line" theme="ovilia-green" ref="line" />
    <p>p1</p>
    <e-charts :options="line" theme="ovilia-green" ref="line" />
    <p>p1</p>
</div>
</template>

<script>
import ECharts from "vue-echarts/components/ECharts";
import "echarts/lib/component/tooltip";
import "echarts/lib/component/legend";
import "echarts/lib/chart/line";

import theme from "./theme.json";

ECharts.registerTheme("ovilia-green", theme);
export default {
    data() {

        return {
            line: {
                // Make gradient line here
                visualMap: [{
                    show: false,
                    type: "continuous",
                    seriesIndex: 1,
                    min: 0,
                    max: 500,
                }, ],
                polar: {
                    center: ["50%", "54%"],
                },
                tooltip: {
                    trigger: "axis",
                },
                xAxis: {
                    data: [
                        1,
                        2,
                        3,
                        4,
                        5,
                        6,
                        7,
                        8,
                        9,
                        10,
                        11,
                        12,
                        13,
                        14,
                        15,
                        16,
                        17,
                        18,
                        19,
                        20,
                        21,
                        22,
                        23,
                        24,
                        25,
                        26,
                        27,
                        28,
                        29,
                        30,
                        31,
                        32,
                        33,
                        34,
                        35,
                        36,
                        37,
                        38,
                        39,
                        40,
                        41,
                        42,
                        43,
                        44,
                        45,
                        46,
                        47,
                        48,
                        49,
                        50,
                        51,
                        52,
                        53,
                        54,
                        55,
                        56,
                        57,
                        58,
                        59,
                        60,
                        61,
                        62,
                        63,
                        64,
                        65,
                        66,
                        67,
                        68,
                        69,
                        70,
                        71,
                        72,
                        73,
                        74,
                        75,
                        76,
                        77,
                        78,
                        79,
                        80,
                        81,
                        82,
                        83,
                        84,
                        85,
                        86,
                        87,
                        88,
                        89,
                        90,
                        91,
                        92,
                        93,
                        94,
                        95,
                        96,
                        97,
                        98,
                        99,
                        100
                    ],
                },
                yAxis: {
                    splitLine: {
                        show: false,
                    },
                },
                series: {
                    type: "line",
                    showSymbol: false,
                    data: [
                        520,
                        536,
                        604,
                        551,
                        568,
                        574,
                        545,
                        576,
                        660,
                        566,
                        533,
                        513,
                        666,
                        525,
                        571,
                        672,
                        519,
                        598,
                        589,
                        445,
                        577,
                        562,
                        548,
                        622,
                        707,
                        611,
                        683,
                        631,
                        603,
                        719,
                        564,
                        680,
                        537,
                        546,
                        716,
                        720,
                        590,
                        638,
                        509,
                        673,
                        507,
                        621,
                        504,
                        510,
                        502,
                        587,
                        733,
                        593,
                        671,
                        600,
                        651,
                        596,
                        580,
                        543,
                        643,
                        678,
                        735,
                        535,
                        752,
                        721,
                        608,
                        715,
                        724,
                        668,
                        656,
                        759,
                        642,
                        708,
                        529,
                        609,
                        674,
                        585,
                        747,
                        555,
                        728,
                        663,
                        762,
                        553,
                        624,
                        522,
                        505,
                        634,
                        597,
                        709,
                        657,
                        776,
                        567,
                        538,
                        71,
                        712,
                        532,
                        527,
                        691,
                        770,
                        746,
                        779,
                        558,
                        701,
                        563,
                        744
                    ],
                },
            },
            line2: {
                // Make gradient line here
                visualMap: [{
                    show: false,
                    type: "continuous",
                    seriesIndex: 1,
                    min: 0,
                    max: 500,
                }, ],
                polar: {
                    center: ["50%", "54%"],
                },
                tooltip: {
                    trigger: "axis",
                },
                xAxis: {
                    data: [101,
                        102,
                        103,
                        104,
                        105,
                        106,
                        107,
                        108,
                        109,
                        110,
                        111,
                        112,
                        113,
                        114,
                        115,
                        116,
                        117,
                        118,
                        119,
                        120,
                        121,
                        122,
                        123,
                        124,
                        125,
                        126,
                        127,
                        128,
                        129,
                        130,
                        131,
                        132,
                        133,
                        134,
                        135,
                        136,
                        137,
                        138,
                        139,
                        140,
                        141,
                        142,
                        143,
                        144,
                        145,
                        146,
                        147,
                        148,
                        149,
                        150,
                        151,
                        152,
                        153,
                        154,
                        155,
                        156,
                        157,
                        158,
                        159,
                        160,
                        161,
                        162,
                        163,
                        164,
                        165,
                        166,
                        167,
                        168,
                        169,
                        170,
                        171,
                        172,
                        173,
                        174,
                        175,
                        176,
                        177,
                        178,
                        179,
                        180,
                        181,
                        182,
                        183,
                        184,
                        185,
                        186,
                        187,
                        188,
                        189,
                        190,
                        191,
                        192,
                        193,
                        194,
                        195,
                        196,
                        197,
                        198,
                        199,
                        200,
                        201,
                        202,
                        203,
                        204,
                        205,
                        206,
                        207,
                        208,
                        209,
                        210,
                        211,
                        212,
                        213,
                        214,
                        215,
                        216

                    ]
                },
                yAxis: {
                    splitLine: {
                        show: false,
                    },
                },
                series: {
                    type: "line",
                    showSymbol: false,
                    data: [628,
                        793,
                        441,
                        514,
                        750,
                        582,
                        625,
                        639,
                        530,
                        756,
                        792,
                        794,
                        791,
                        516,
                        632,
                        670,
                        706,
                        795,
                        796,
                        775,
                        800,
                        736,
                        801,
                        601,
                        654,
                        751,
                        808,
                        802,
                        688,
                        741,
                        710,
                        818,
                        813,
                        584,
                        807,
                        524,
                        575,
                        766,
                        544,
                        821,
                        518,
                        722,
                        616,
                        777,
                        644,
                        696,
                        758,
                        665,
                        623,
                        540,
                        717,
                        803,
                        698,
                        677,
                        755,
                        764,
                        773,
                        512,
                        556,
                        740,
                        713,
                        552,
                        528,
                        686,
                        303,
                        761,
                        765,
                        830,
                        797,
                        517,
                        694,
                        588,
                        831,
                        850,
                        697,
                        581,
                        586,
                        655,
                        734,
                        560,
                        826,
                        617,
                        633,
                        703,
                        784,
                        561,
                        635,
                        324,
                        652,
                        506,
                        645,
                        627,
                        702,
                        618,
                        647,
                        653,
                        730,
                        783,
                        820,
                        853,
                        859,
                        863,
                        869,
                        871,
                        653,
                        783,
                        730,
                        863,
                        647,
                        869,
                        859,
                        853,
                        820,
                        875,
                        884,
                        833,
                        824,
                        547,
                        439,
                        782,
                        679,
                        711,
                        605,
                        629,
                        874,
                        675
                    ],
                },
            },

        };
    },
    components: {
        ECharts,
    },
};
</script>
