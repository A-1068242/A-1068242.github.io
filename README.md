[github.html](https://github.com/user-attachments/files/27172499/github.html)
<!DOCTYPE html>
<html lang="zh-CN">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>标量工程 · 从试验田到全景图</title>
<style>
  *{margin:0;padding:0;box-sizing:border-box}
  body{
    background:#f2efe9;
    color:#3a3a3a;
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", "PingFang SC", "Microsoft YaHei", sans-serif;
    line-height:1.8;
    -webkit-font-smoothing:antialiased;
  }
  .container{max-width:800px;margin:0 auto;padding:60px 24px 80px}

  /* 顶部标题区 */
  .masthead{
    border-left:4px solid #ff4c00;
    padding-left:20px;
    margin-bottom:60px;
  }
  .masthead .slug{
    font-size:13px;
    letter-spacing:3px;
    color:#8a8a8a;
    text-transform:uppercase;
    margin-bottom:8px;
  }
  .masthead h1{
    font-size:28px;
    font-weight:600;
    color:#1c1c1c;
    letter-spacing:1px;
  }
  .masthead .sub{
    margin-top:10px;
    font-size:14px;
    color:#6a6a6a;
  }

  /* 分隔线 */
  .divider{
    height:1px;
    background:#dcd8d0;
    margin:50px 0;
    position:relative;
  }
  .divider::after{
    content:"";
    position:absolute;
    left:0;
    top:-2px;
    width:24px;
    height:4px;
    background:#ff4c00;
  }

  /* 章节标题 */
  .section-title{
    font-size:18px;
    font-weight:600;
    color:#1c1c1c;
    margin-bottom:20px;
    padding-left:14px;
    border-left:3px solid #ff4c00;
  }

  /* 正文段落 */
  p{margin-bottom:18px;font-size:15px;color:#4a4a4a}
  .note{font-size:13px;color:#8a8a8a;font-style:italic}

  /* 问题列表 */
  .issue-list{
    list-style:none;
    margin:16px 0 24px;
  }
  .issue-list li{
    padding:8px 0 8px 20px;
    position:relative;
    font-size:14px;
    color:#4a4a4a;
  }
  .issue-list li::before{
    content:"";
    position:absolute;
    left:0;
    top:16px;
    width:6px;
    height:6px;
    background:#ff4c00;
    border-radius:1px;
  }

  /* 行动列表 */
  .action-list{
    list-style:none;
    counter-reset:step;
    margin:16px 0 24px;
  }
  .action-list li{
    counter-increment:step;
    padding:10px 0 10px 32px;
    position:relative;
    font-size:14px;
    color:#4a4a4a;
  }
  .action-list li::before{
    content:counter(step);
    position:absolute;
    left:0;
    top:10px;
    width:20px;
    height:20px;
    background:#3a3a3a;
    color:#f2efe9;
    font-size:11px;
    font-weight:600;
    text-align:center;
    line-height:20px;
    border-radius:1px;
  }

  /* 过渡区 */
  .transition-block{
    background:#ffffff;
    border:1px solid #dcd8d0;
    padding:32px 28px;
    margin:40px 0;
    position:relative;
  }
  .transition-block .tag{
    display:inline-block;
    background:#ff4c00;
    color:#fff;
    font-size:11px;
    letter-spacing:2px;
    padding:4px 10px;
    margin-bottom:16px;
    border-radius:1px;
  }
  .transition-block .big-q{
    font-size:16px;
    font-weight:600;
    color:#1c1c1c;
    margin-bottom:16px;
    line-height:1.6;
  }
  .transition-block .arrow-down{
    text-align:center;
    margin:20px 0 8px;
    color:#ff4c00;
    font-size:20px;
    letter-spacing:4px;
  }

  /* 集团卡片网格 */
  .card-grid{
    display:grid;
    grid-template-columns:1fr 1fr;
    gap:16px;
    margin:24px 0;
  }
  @media(max-width:600px){.card-grid{grid-template-columns:1fr}}
  .card{
    background:#fff;
    border:1px solid #dcd8d0;
    padding:20px;
    border-radius:1px;
    transition:border-color .2s;
  }
  .card:hover{border-color:#ff4c00}
  .card .num{
    font-size:11px;
    color:#8a8a8a;
    letter-spacing:2px;
    margin-bottom:6px;
  }
  .card .name{
    font-size:16px;
    font-weight:600;
    color:#1c1c1c;
    margin-bottom:4px;
  }
  .card .eng{
    font-size:11px;
    color:#8a8a8a;
    text-transform:uppercase;
    letter-spacing:1px;
    margin-bottom:10px;
  }
  .card .desc{
    font-size:13px;
    color:#5a5a5a;
    line-height:1.6;
  }

  /* 底部注记 */
  .footer-note{
    margin-top:50px;
    padding-top:30px;
    border-top:1px solid #dcd8d0;
    font-size:12px;
    color:#8a8a8a;
    text-align:center;
  }
  .footer-note span{
    color:#ff4c00;
  }
</style>
</head>
<body>
<div class="container">

  <!-- ===== 顶部标题 ===== -->
  <div class="masthead">
    <div class="slug">标量工程 · 项目展示</div>
    <h1>从试验田到全景图</h1>
    <div class="sub">一个方法论在两种尺度下的推演</div>
  </div>

  <!-- ===== 第一部分：校园小卖部 ===== -->
  <div class="section-title">一、项目缘起：校园微型零售服务站</div>
  <p>高校校园是典型的半封闭消费市场，学生日均消费频次高、品类需求稳定，但校内零售业态长期呈现碎片化与低效化。我们在前期观察中发现三个具体问题：</p>
  <ul class="issue-list">
    <li>超市、自动售货机、线上外卖各自为战，品类割裂、消费场景彼此孤立。</li>
    <li>各零售主体在选品、定价、服务规范上缺乏协同，品质参差、价格浮动无序。</li>
    <li>学生无法积累对任何一家校内零售主体的稳定信任，消费决策成本居高不下。</li>
  </ul>
  <p>这些问题很小，但揭示了一个被忽视的命题：<strong>即便在最微小的零售场景里，跨品类、跨终端的标准化协同也是一个真问题。</strong></p>

  <div class="divider"></div>

  <div class="section-title">二、项目内容</div>
  <p>本项目拟在校内试点一个“校园微型零售服务站”，核心动作四项：</p>
  <ol class="action-list">
    <li>发放不少于200份问卷，建立高频消费品类的需求频次与价格敏感度图谱。</li>
    <li>制定《校园零售服务站选品标准与定价规则》，覆盖食品、日用品、电子配件三大品类，建立统一准入编码、品质分级与价格浮动标准。</li>
    <li>在实体货架、自动售货柜、线上预订端口三个消费触点之间统一商品陈列、价签样式与服务说明。</li>
    <li>依据标准反向筛选供应商，建立跨品类联合采购清单与库存共享规则，通过短期试运营评估标准化在小微场景中的成本效益边界。</li>
  </ol>
  <p class="note">这并非简单的“开一家小卖部”，而是一次“最小可行规模”的方法论在地测试。</p>

  <div class="divider"></div>

  <!-- ===== 过渡区 ===== -->
  <div class="transition-block">
    <div class="tag">过渡</div>
    <p style="font-size:14px;color:#5a5a5a;margin-bottom:12px;">申报书里的校园小卖部，是一次方法论的在地测试。我们想验证：<strong>“先定标准、再组货架、统一终端”</strong>这套逻辑，在最小规模的零售场景里能否跑通。</p>
    <div class="big-q">如果这套逻辑跑通了，把它放大一百倍，放进一个真正的多产业企业集团里，它应该长成什么样子？</div>
    <p style="font-size:14px;color:#5a5a5a;">小卖部的“跨品类选品标准”，逻辑上等同于集团层面的“跨业务单元协同标准”；小卖部多终端的统一陈列与服务，逻辑上等同于集团各子公司输出一致性的管控体系；小卖部的联合采购与库存共享，逻辑上等同于集团供应链的资源整合与规模效应释放。</p>
    <p style="font-size:14px;color:#1c1c1c;font-weight:600;margin-top:12px;">问题同构，方法同源。我们将同一套方法论外推至跨行业、跨品类的完整商业生态——这个外推的沙盘，命名为“标量工程”。</p>
  </div>

  <div class="divider"></div>

  <!-- ===== 第三部分：集团架构 ===== -->
  <div class="section-title">三、标量工程 · 集团架构</div>
  <p>以下六家子公司覆盖能源、工业、交通、电子、零售、食药六大产业板块，共享同一套协同标准体系。</p>

  <div class="card-grid">
    <div class="card">
      <div class="num">01</div>
      <div class="name">辉光科技</div>
      <div class="eng">Consumer Electronics</div>
      <div class="desc">负责个人计算终端、智能移动设备及周边配件的工业设计与全渠道销售，承担体系内电子类产品的统一设计标准制定。</div>
    </div>
    <div class="card">
      <div class="num">02</div>
      <div class="name">标准食品</div>
      <div class="eng">Food &amp; Retail</div>
      <div class="desc">主营谷物加工、生鲜果蔬直供及日用快消品开发，实行统一采购、统一包装、统一品控管理模式。</div>
    </div>
    <div class="card">
      <div class="num">03</div>
      <div class="name">XX集团</div>
      <div class="eng">Metals &amp; Machinery</div>
      <div class="desc">涵盖有色金属选矿冶炼、合金材料研发与大型工程机械制造，承担体系内各子公司定制合金与金属原料的定向供应。</div>
    </div>
    <div class="card">
      <div class="num">04</div>
      <div class="name">西部交建</div>
      <div class="eng">Rail Transit</div>
      <div class="desc">主营有轨电车与市域动车组整车设计装配，提供车辆段级维护及技术升级服务。</div>
    </div>
    <div class="card">
      <div class="num">05</div>
      <div class="name">北方电筹</div>
      <div class="eng">Energy &amp; Grid</div>
      <div class="desc">运营集中式光伏电站、储能设施建设与区域配电网调度，负责所辖范围内工业及民用电力稳定供应。</div>
    </div>
    <div class="card">
      <div class="num">06</div>
      <div class="name">北极点生物制药公司</div>
      <div class="eng">Biomedicine</div>
      <div class="desc">涵盖处方药生产、功能性营养剂开发与医用生物材料研究，承担体系内食品药品安全检测标准的制定与验证。</div>
    </div>
  </div>

  <div class="divider"></div>

  <!-- ===== 设计宪法摘要 ===== -->
  <div class="section-title">四、设计宪法 · 节选</div>
  <p style="font-size:14px;color:#5a5a5a;">以下为标量工程体系内所有子公司共同遵循的设计约束：</p>
  <table style="width:100%;border-collapse:collapse;margin-top:12px;font-size:13px;">
    <tr style="border-bottom:1px solid #dcd8d0;">
      <td style="padding:10px 8px;color:#1c1c1c;font-weight:600;width:30%;">主色</td>
      <td style="padding:10px 8px;color:#4a4a4a;">哑光深灰 #3A3A3A / 哑光暖白 #F2EFE9 / 哑光黑 #1C1C1C</td>
    </tr>
    <tr style="border-bottom:1px solid #dcd8d0;">
      <td style="padding:10px 8px;color:#1c1c1c;font-weight:600;">信号色</td>
      <td style="padding:10px 8px;color:#4a4a4a;">荧光橙 #FF4C00（仅用于安全标识、关键触点和比例强调）</td>
    </tr>
    <tr style="border-bottom:1px solid #dcd8d0;">
      <td style="padding:10px 8px;color:#1c1c1c;font-weight:600;">几何规则</td>
      <td style="padding:10px 8px;color:#4a4a4a;">所有产品造型必须可归纳为基本几何体或其布尔运算结果</td>
    </tr>
    <tr>
      <td style="padding:10px 8px;color:#1c1c1c;font-weight:600;">禁止项</td>
      <td style="padding:10px 8px;color:#4a4a4a;">禁止随机曲线、无意义的装饰纹样、与功能无关的色彩添加</td>
    </tr>
  </table>

  <!-- ===== 底部 ===== -->
  <div class="footer-note">
    <p>本项目为创新创业课程模拟作业。校园微型零售服务站为申报阶段内容；标量工程集团架构为<strong>同一方法论的原则性外推</strong>，属沙盘推演性质。</p>
    <p style="margin-top:6px;"><span>SCALAR ENGINEERING</span> · 为混乱的物理世界建立统一的设计秩序</p>
  </div>

</div>
</body>
</html>
