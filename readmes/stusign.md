<!-- markdownlint-disable MD031 MD033 MD036 -->

# StuSign

简洁的签到插件

## 介绍

### Features

_自用插件，功能虽然比不上论坛里的其它插件，但就是图简洁，满足自己需求_

- 入服签到，并在**聊天栏**提醒，不挡公告
- 对接 LLMoney
- 每次签到随机给钱，可配置

## 安装方法

将 `StuSign.lls.js` 扔进 BDS 插件目录即可

## 配置文件

插件配置文件位于`BDS根目录/plugins/StuSign/config.json`（插件加载成功后自动生成）  
请根据下面 json 中的注释修改配置文件

```jsonc
{
  // 签到给予最少金钱数
  "minMoney": 500,

  // 签到给予最多金钱数
  "maxMoney": 2000
}
```

## 联系我

QQ：3076823485  
吹水群：[1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp)  
邮箱：<lgc2333@126.com>

## 赞助

感谢大家的赞助！你们的赞助将是我继续创作的动力！

- [爱发电](https://afdian.net/@lgc2333)
- <details>
    <summary>赞助二维码（点击展开）</summary>

  ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)

  </details>

## 更新日志

- 0.1.1
  - 添加每天 0:00 自动给所有服务器内玩家签到
