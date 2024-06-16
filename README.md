## 置顶公告

公告

从2024/6/5号开始如果宣传了JSDMirror可以带上你的博客和截图,在网站联系uid为1或者是发送邮件kefu@cola.email 根据内容换取500-5000积分+1年平台会员大概可以清理1000次缓存缓存，活动结束日期2025年6月30号，每一个网站，每一个主体备案号只能参加一次，发过一次的话可以重新发的哦

公告2
免审核的jsdmirror上线了
*.cdn.xzzo.cn
一，
去console.xzzo.cn，完成注册并搞基础实名认证后。即可向管理员申请
对应网站需要悬挂
	<a href="https://www.jsdmirror.com">页面资源由jsdmirror提供</a>具体看你使用什么，在你的网站下悬挂。

二，
这个是自定义页面 在我们提供的域名下悬挂

1.允许自定义域名前缀

2.允许自定义静态页面,包含php,代码禁止混淆,加密,要求代码能够正常阅读理解 php8语法，如有报错则审核不通过。禁止连接任何形式的数据库和数据库

需要在底部悬挂。<a href="https://www.zeyao.net">泽瑶网络</a>
授权
<a href="https://你网站">你网站名字 </a>使用
&copy; 2023-2024 你网名 All Rights Reserved.
<div>
本系统有：
<a href="https://www.zzko.cn">泽瑶静态资源站</a> · <a href="https://www.ayao.ltd">阿瑶の Blog</a> · <a href="https://www.jsdmirror.com">jsdelivr镜像站</a>提供</div>

  <a href="https://beian.miit.gov.cn" id="miit"  target="_blank">辽ICP备2023005487号-8</a> | <a href="https://beian.mps.gov.cn/#/query/webSearch?recordcode=2102810200xxxx" id="miit"  target="_blank">辽公网安备2102810200xxxx号</a> (后续会通知你更新的)| 
<a href="https://icp.gov.moe/?keyword=2024xxxx" target="_blank">萌ICP备2022xxx号</a>(需要自行申请)
  
<p>本站不提供任何视听上传存储服务，所有内容均来自Jsdelivr站点提供的公开引用资源。进行分发服务<br>如存在版权或非法内容，欢迎举报，我们将尽快予以屏蔽<br>举报邮箱: kefu@cola.email 我们将于1-3个工作日受理举报您的举报<p>网上有害信息举报专区：<i class="sprite bg3"></i><a href="https://www.12377.cn/" target="_blank">中国互联网违法和不良信息举报中心</a><br>
网络犯罪举报专区：<i class="sprite bg3"></i><a href="http://cyberpolice.mps.gov.cn/wfjb/" target="_blank">网络犯罪举报中心</a></p>

内容是这样的但是格式不限制。

主要悬挂这几个 每行顺序不限， 需要同时满足

公告3
平台近期发现大量ts切片视频，指向了某一个二次元网站，占用的流量比较多，主要也没什么问题经审核视频中存在不良广告，主要是广告违反了我们的tos，经评估研究决定，平台即禁止加速 ts m3u8 （2024-7-1）正式执行，在此之间 上述文件将限速 1024/kb 如果有上述资源，请尽快迁移完成


## 项目介绍


本项目自2021年12月21日上线以来，原由54ayao（Eagle Yao）运营和维护。经过数轮版本迭代，现已交由大连市泽瑶网络科技有限公司负责运营。JSDMirror致力于为广大开发者提供免费的CDN加速服务，通过优化网站加速、应用程序优化等多种场景，提升用户体验。
我们已启用全新架构 cdn.JSDMirror.com为你提供服务
请大家尽快完成更换，如果不需要更换的话，请提交is进行排除。谢谢

## 核心功能

1. **高速镜像站**

我们现采用腾讯云中国香港Tencent Kubernetes Engine作为源站，根据网站流量来自动提升服务器

参考此类技术文章

https://mp.weixin.qq.com/s/o9giQ3efqvNG9FQe0LM35A


2. **多融合cdn**

我们使用的cdn供应商有

境内
白山CDN，腾讯云CDN, 腾讯云EO,百度CDN,阿里DCDN,华为CDN,天翼边缘加速，网宿CDNPro, 

海外
cloudflare、CDNetWorks、Tencent Cloud、bunny、 Vercel  

平台根据运营情况自动决定cdn供应商

3. **免费性**

提供免费的CDN服务，用户只需把jsdelivr官方域名转换成jsdmirror域名即可使用。这一特点降低了开发者的成本负担，使得更多的开发者能够享受到CDN带来的加速效果

4. **冗余部署**

jsdmirror采用了多节点冗余部署的策略。这意味着，不是所有的用户请求都会发送到同一个服务器上，而是会被分散到多个地理位置的服务器上。这样，即使某个服务器出现故障，其他服务器也能接管请求，确保服务的连续性。

5. **负载均衡**

除了冗余部署，jsdmirror还使用了先进的负载均衡技术。这种技术能够根据服务器的负载情况，动态地分配用户请求。这样，即使在高流量时段，也能确保每个服务器的负载保持在合理水平，避免单个服务器过载而导致的宕机。

6. **故障自动恢复**

jsdmirror的监控系统会实时监测所有服务器的状态。一旦发现某个服务器出现故障，腾讯云IGTM监控系统会立即触发自动恢复流程。切换到备用服务器或CDN等措施，以确保服务尽快恢复正常。

7. **数据备份与同步**

为了防止数据丢失，jsdmirror还采取了数据备份和同步的策略。所有存储在COS上的数据都会在多个地理位置进行备份。同时，这些备份数据会实时同步，确保无论在哪个地理位置的服务器出现问题，都能够从最近的备份中恢复数据。

8. **灵活定制**

用户可以根据自身需求，自定义CDN加速规则，实现精细化运营。例如，针对特定文件类型或地区进行优化，以满足用户的个性化需求。

9. **实时监控**

jsdmirror提供了实时监控功能，用户可以随时查看CDN的运行状态和性能指标。这有助于用户及时发现并解决问题，确保服务的稳定运行。

10. **安全保障**

jsdmirror注重用户数据安全，采用了多重加密技术和严格的安全策略。用户的数据在传输和存储过程中都得到了充分保护，有效防止了数据泄露和恶意攻击。


## JSDMirror的应用场景

1. 开源项目加速

对于开发者而言，JSDMirror可以显著提升开源项目的下载速度和稳定性，助力开源社区的发展。

2. 网站加速

通过使用JSDMirror，网站管理员可以将静态资源部署到CDN上，实现网站的快速加载和流畅访问。


3. 内容分发：内容创作者可以利用JSDMirror将内容分发到全球各地，扩大影响力并吸引更多用户。


根据有关部门要求，我们对平台协议进行了更新。

## 遵守平台规定

根据中华人民共和国工业和信息化部、公安部等部委关于加强在公共信息服务中传播信息管理的有关规定和相关精神，要求各单位落实完毕

一、不利用像站危害国家安全、泄露国家秘密，不侵犯国家的、社会的、集体的利益和第三方的合法权益，不从事违法犯罪活动、妨碍社会治安的活动。

1.煽动抗拒、破坏宪法和法律、行政法规实施的；

2.煽动颠覆国家主权，推翻社会主义制度的；

3.煽动分裂国家、破坏国家统一的;

4.煽动民族仇恨、民族歧视，破坏民族团结的；

5.捏造或者歪曲事实，散布谣言，扰乱社会秩序的；

6.宣传封建迷信、淫秽、色情、赌博、暴力、凶杀、恐怖犯罪的；

7.公然侮辱他人或者捏造事实诽谤他人的；

8.损害国家机关信誉的;

9.传播不实信息，危害或对社会安全行为造成恐慌

10.其它违反宪法和法律、行政法规的。

二、色情低俗类

1.表现或隐晦表现性行为、令人产生性联想、具有挑逗性或者污辱性的内容；

2.对人体性部位的直接暴露和描写；

3.对性行为、性过程、性方式的描述或者带有性暗示、性挑逗的语言；

4.对性部位描述、暴露，或者只用很小遮盖物的内容；

5.全身或者隐私部位未着衣物，仅用肢体掩盖隐私部位的内容；

6.带有侵犯个人隐私性质的走光、偷拍、漏点等内容：

7.以挑逗性标题吸引点击的；

8.相关部门禁止传播的色情、低俗小说，音视频内容，包括一些电影的删节片断；

9.一夜情、换妻、SM等不正当交友信息；

10.情色动漫，(以露点或者是以漏点用小幅度遮挡为判断)；

11.宣扬血腥暴力、恶意谩骂、侮辱他人等内容；

12.非法性用品广告和性病治疗广告：

13.为经他人允许或利用“人肉搜索”恶意传播他人隐私信息。

三、不得从事下列危害计算机信息网络安全的活动，包括但不限于：

1.未经允许，进入计算机信息网络或者使用计算机信息网络资源的：

2.未经允许，对计算机信息网络功能进行删除、修改或者增加的：

3.末经允许，对计算机信息网络中存储、处理或者传输的数据和应用程序进行删除、修改或者增加的:

4.故意制作、传播计算机病毒等破坏性程序的:

5.其他危害计算机信息网络安全的。

四、承诺在镜像站上播发的信息内容是经当当地宜传管理部门符合/批准的允许内容


五、补充协议

1.反正内容需合法合规

2.不得应用到违规网站，尤其是灰黑产业，不符合工信部或者当地国家规定的项目（

3.项目支持下载，但不能下载违反国家法律法规，你要用就悄咪咪的用，别通过这个链接分享，不该我真的栓Q， 国际站除外

4.未经许可不得再次反向代理该网站 或者反向代理我源站进行二次分发

5.github 项目在不违规的不做任何屏蔽的目的是为了更好的用户体验，麻烦你们不要把我搞得像jsd一样被污染一段时间

6.如果触发防火墙，代表你IP一分钟已经超过2000次，被防火墙的屏蔽被两个三小时之后再试，家庭用户可尝试重启路由器来获取新的IP。或者是保持正常访问。

7.未经允许严禁使用回源其包括但不限于中国香港，新加坡，中国台湾，泰国，孟买，美国，日本，韩国，中国广州，中国成都，中国宿迁，中国杭州，等  cdn.jsdmirror.com和cdn.jsdmirror.cn jsd.cdn.zzko.cn 以及 cdn.jsdelivr.us www.jsdelivr.ren 和*.cdn.xzzo.cn 以及jsd.cdn.zzko.cn源站集群，

8.您需要理解我们基于合规性每个月不定期都会从cdn平台抽取日志进行抽查，因为大部分流量都不发送请求域名，我们参考加速项目URL地址来

## 平台管理员联系方式与问题反馈 

反馈渠道
微信>>企业微信>企业微信邮件>tg>QQ>bilibili

|QQ|企业微信|github|TG|邮箱|
|-------|---------------|----------|------|------|
|202835956|<img src="https://github.com/54ayao/JSDMirror/assets/86733666/aa633562-1b3b-438e-868b-15c0b5a445bd" alt="企业微信">|[点这里](https://github.com/54ayao/JSDMirror/issues) |[点这里](https://t.me/jsdmirrorChannel)|ayao@cola.email|



可能出现解封的机会

![image](https://github.com/54ayao/JSDMirror/assets/86733666/d80c0729-8d4c-4107-96fa-0ef8332bc99b)

如果出现这个情况请联系管理员进行处理


![image](https://github.com/54ayao/JSDMirror/assets/86733666/54c1303f-a229-498f-9774-3f7879a0c134)

如红框所示，某一些太过分的就没办法解封了，还有可能影响到你整个用户

![image](https://github.com/54ayao/JSDMirror/assets/86733666/6b283f22-de90-473c-9378-5912c914f94b)
如果出现这个情况请联系管理员进行询问是什么违规

说明：

1.平台发现部分人使用多个//绕过封禁系统，达到继续使用的目的 ，在这里我们联系CDN供应商特殊配置修复了使用多个//绕过封禁系统的BUG（目录侧输入大于等于俩个/ 系统按一个计算）


(被审核系统处理了一定要跟我说 我第一时间处理！！！不要哑不吭声的，到头来日志被覆盖了，很麻烦的)


赞助可以选择服务器，CDN，域名费用，cdn费用，审核费用，赞助和广告位挂钩，不存在购买广告位 比如说你赞助每个月赞助2tb cdn 假设为1年 我们会在判断节点覆盖率并在合理位置悬挂广告1年 服务器看配置 建议20mpbs 以上的按量无所谓的 也可以