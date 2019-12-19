<template>
    <div>
        <h1>电影排行榜</h1>
        <h2 style="color:#072;width:160px;">新片榜   · · · · · · </h2>
        <div style="border-top:1px dashed #cccccc;height:1px;overflow:hidden"></div>

        <el-row type="flex" justify="center" :gutter="20">
            <el-col :span="2">
                <img src="../assets/6.jpg" style="width:110px;height:160px;margin-top:23px;">
            </el-col>
            <el-col style="text-align: left;margin-left:50px; ">
                <div style="color:#37a;margin-top:25px;">
                    {{movie1.title}}
                </div>
                <div style="margin-top:23px">
                    {{movie1.text}}
                </div>
                <div style="margin-top: 5px;">
                    <el-col style="text-align: left">
                        <div style="display: inline-block ">
                            <el-rate disabled v-model="movie1.scoring.star"></el-rate>
                                <div style="font-size: 12px;padding-left: 3px">{{movie1.scoring.amount}}个人评价</div>
                        </div>
                    </el-col>
                </div>
            </el-col>
        </el-row>

        <div style="border-top:1px dashed #cccccc;height:1px;overflow:hidden"></div>
        <el-row type="flex" justify="center" :gutter="20">
            <el-col :span="2">
                <img src="../assets/1.jpg" style="width:110px;height:160px;margin:23px;">
            </el-col>
            <el-col style="text-align: left;margin-left:50px; ">
                <div style="color:#37a;margin-top:25px;">
                    {{movie2.title}}
                </div>
                <div style="margin-top:23px">
                    {{movie2.text}}
                </div>
                <div style="margin: 5px;">
                    <el-col style="text-align: left">
                        <div style="display: inline-block ">
                            <el-rate disabled v-model="movie2.scoring.star">
                                <div style="font-size: 12px;padding-left: 3px">{{movie2.scoring.amount}}个人评价</div>
                            </el-rate>
                        </div>
                    </el-col>
                </div>
            </el-col>
        </el-row>

        <div style="border-top:1px dashed #cccccc;height:1px;overflow:hidden"></div>
        <el-row type="flex" justify="center" :gutter="20">
            <el-col :span="2">
                <img src="../assets/2.jpg" style="width:110px;height:160px;margin:23px;">
            </el-col>
            <el-col style="text-align: left;margin-left:50px; ">
                <div style="color:#37a;margin-top:25px;">
                    {{movie3.title}}
                </div>
                <div style="margin-top:23px">
                    {{movie3.text}}
                </div>
                <div style="margin: 5px;">
                    <el-col style="text-align: left">
                        <div style="display: inline-block ">
                            <el-rate disabled v-model="movie3.scoring.star">
                                <div style="font-size: 12px;padding-left: 3px">{{movie3.scoring.amount}}个人评价</div>
                            </el-rate>
                        </div>
                    </el-col>
                </div>
            </el-col>
        </el-row>

        <div style="border-top:1px dashed #cccccc;height:1px;overflow:hidden"></div>
        <el-row type="flex" justify="center" :gutter="20">
            <el-col :span="2">
                <img src="../assets/8.jpg" style="width:110px;height:160px;margin:23px;">
            </el-col>
            <el-col style="text-align: left;margin-left:50px; ">
                <div style="color:#37a;margin-top:25px;">
                    {{movie4.title}}
                </div>
                <div style="margin-top:23px">
                    {{movie4.text}}
                </div>
                <div style="margin: 5px;">
                    <el-col style="text-align: left">
                        <div style="display: inline-block ">
                            <el-rate disabled v-model="movie4.scoring.star">
                                <div style="font-size: 12px;padding-left: 3px">{{movie4.scoring.amount}}个人评价</div>
                            </el-rate>
                        </div>
                    </el-col>
                </div>
            </el-col>
        </el-row>
    </div>
</template>
<script>
    export default {
        data(){
            return {
                movie1: {
                    title: "爱尔兰人 / 爱尔兰杀手(港) / 听说你刷房子了",
                    text: "2019-09-27(纽约电影节) / 2019-11-01(美国点映) / 2019-11-27(美国网络) / 罗伯特·德尼罗 / 阿尔·帕西诺 / 乔·佩西 / 安娜·帕奎因 / 杰西·普莱蒙 / 哈威·凯特尔 / 斯蒂芬·格拉汉姆 / 鲍比·坎纳瓦尔 / 杰克·休斯顿 / 阿莱卡萨·帕拉迪诺 / 凯瑟琳·纳杜奇...",
                    scoring: {
                        amount: 378978,
                        star: 4.5
                    }
                },
                movie2: {
                    title: "小丑 / 小丑起源电影：罗密欧 / Romeo",
                    text: "2019-08-31(威尼斯电影节) / 2019-10-04(美国) / 杰昆·菲尼克斯 / 罗伯特·德尼罗 / 马克·马龙 / 莎姬·贝兹 / 谢伊·惠格姆 / 弗兰西丝·康罗伊 / 布莱恩·考伦 / 布莱恩·泰里·亨利 / 布莱特·卡伦 / 道格拉斯·霍奇斯 / 格伦·弗莱施勒 / 比尔·坎普...",
                    scoring: {
                        amount: 380742,
                        star: 3.5
                    }
                },
                movie3: {
                    title: "好莱坞往事 / 从前，有个荷里活(港) / 从前，有个好莱坞...(台)",
                    text: "2019-05-21(戛纳电影节) / 2019-07-26(美国) / 2019(中国大陆) / 莱昂纳多·迪卡普里奥 / 布拉德·皮特 / 玛格特·罗比 / 埃米尔·赫斯基 / 玛格丽特·库里 / 蒂莫西·奥利芬特 / 茱莉亚·巴特斯 / 奥斯汀·巴特勒 / 达科塔·范宁 / 布鲁斯·邓恩 /...",
                    scoring: {
                        amount: 286847,
                        star: 4
                    }
                },
                movie4: {
                    title: "准备好了没 / 弑婚游戏(台) / 爆血新婚夜(港)",
                    text: "2019-08-21(美国) / 萨玛拉·维文 / 安迪·麦克道威尔 / 马克·奥布莱恩 / 亚当·布罗迪 / 亨利·科泽尼 / 妮基·瓜达尼 / 梅兰妮·斯科洛凡诺 / 克里斯蒂安·布鲁恩 / 伊利斯 莱韦斯克 / 约翰·拉尔斯顿 / 达妮埃拉·巴博萨 / 伊拉娜·盖尔 /...",
                    scoring: {
                        amount: 26708,
                        star: 3
                    }
                }
            }
        }
    }
</script>
<style scoped>
    h1 {
        margin-top: 50px;
        word-wrap: break-word;
        display: block;
        font-size: 30px;
        font-weight: bold;
        color: #494949;
        padding: 0 0 15px 0;
        line-height: 1.1;
        text-align: left;
    }

</style>