# jd_maotai rpa
基于selenium驱动的jd抢购rpa机器人, 照顾我们这样的马大哈, 不会忘记抢购了, 祝大家过年都能喝上茅台.

## 特别声明:

* 本仓库发布的`jd_maotai_rpa`项目定义为自动化rpa项目, 是用于防止忘记参与jd茅台的活动(由于本人时常忘记), 而不是为了秒杀和抢购。

* 本仓库发布的`jd_maotai_rpa`项目中涉及的任何脚本，仅用于测试和学习研究，禁止用于商业用途，不能保证其合法性，准确性，完整性和有效性，请根据情况自行判断。

* 本项目内所有资源文件，禁止任何公众号、自媒体进行任何形式的转载、发布。

* `zhaoxilingcheng` 对任何脚本问题概不负责，包括但不限于由任何脚本错误导致的任何损失或损害.

* 间接使用脚本的任何用户，包括但不限于建立VPS或在某些行为违反国家/地区法律或相关法规的情况下进行传播, `zhaoxilingcheng` 对于由此引起的任何隐私泄漏或其他后果概不负责。

* 请勿将`jd_maotai_rpa`项目的任何内容用于商业或非法目的，否则后果自负。

* 如果任何单位或个人认为该项目的脚本可能涉嫌侵犯其权利，则应及时通知并提供身份证明，所有权证明，我们将在收到认证文件后删除相关脚本。

* 以任何方式查看此项目的人或直接或间接使用`jd_maotai_rpa`项目的任何脚本的使用者都应仔细阅读此声明。`zhaoxilingcheng` 保留随时更改或补充此免责声明的权利。一旦使用并复制了任何相关脚本或`jd_maotai_rpa`项目，则视为您已接受此免责声明。
  
* 您必须在下载后的24小时内从计算机或手机中完全删除以上内容。  
  
* 本项目遵循`GPL-3.0 License`协议，如果本特别声明与`GPL-3.0 License`协议有冲突之处，以本特别声明为准。

> ***您使用或者复制了本仓库且本人制作的任何代码或项目，则视为`已接受`此声明，请仔细阅读***  
> ***您在本声明未发出之时点使用或者复制了本仓库且本人制作的任何代码或项目且此时还在使用，则视为`已接受`此声明，请仔细阅读***

## 说明
我认为直接采用selenium驱动的参与抢购活动更直观, 问题少, 实现简单, 然而不会存在十全十美的办法, 此方式的实现导致抢购速度不如requests请求来的快, 但好在不需要参考太多参数, 不需要一点一点的去抓包分析.

## 实现说明
1. 用户扫码直接登录
2. 计算jd与本地时差
3. 提前刷新页面监控字段值
4. 点击具体的字段值
5. 如果可以提交订单则提交订单
6. 否则失败

