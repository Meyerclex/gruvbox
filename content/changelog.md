---
title: 💎站点更新日志 Changelog
description:
date: 2021-06-28
slug: changelog
---

<style>
.article-header {
    display: none;
  }
.article-footer {
	display: none;
  }
</style>

## 💎 站点更新日志

#### 2022-09-14

文章页面打开时实在过分卡顿，排查原因，查到[一篇文章](https://segmentfault.com/a/1190000002970056)谈到是背景图片显示方式`background-attachment: fixed;`导致的，一口气注释掉。

原文提供的优化方法试了几次都会导致字重显示有误（怀疑是`::before`的原因），最终也没有找到能够让图片不滚动的方法，图片滚动好像又会导致渲染不及时所以下滑时有短暂的大闪白光效果（）？，所以加了一行`will-change: auto;`应付一下就算完事了，谁知道起不起效果，不管你了！

不知道为什么表情变得奇大无比，于是修改了评论区表情的大小和显示方式，现在悬停在它们身上可以获得放大效果，超可爱。感谢[咖啡冰河的文章](https://blog.mysto.cyou/posts/211028-blognewtheme/)：

```
    img.wl-emoji,
    img.vemoji {
        width: 38px;
        vertical-align: sub;
        transition: ease-out .6s;
    }

    img.wl-emoji:hover,
    img.vemoji:hover {
        transform: scale(1.75);
    }
```

#### 2022-09-10

由于 Luna 实在难以驾驭，所以换回了又快又好用的 Stack 主题噗哈哈哈 XD！对主题一番装修，人家的 CSS 知识还没法照顾到移动端的适配，希望不要出太大差错。

#### 2022-08-30

取消了 Channel.io 聊天气泡.

#### 2022-07-24

根据芋阿圆的笔记增加了文章段首空两格的 Feature.

#### 2022-05-24

终于把消失很久的聊天小气泡加上，虽然没有人找我聊天啦 💬

#### 2022-05-22

终于把页脚的心头大患 Run Time 给改了实现了所有想要的 Feature 了，小鸟立誓再也不会打开装修页面了 😤VS code 也卸载了（假的），再见！

#### 2022-05-19

经过爆破艰难地更新了船新版本的 Luna，获取了浮动 Toc 并立誓再也不更新主题了

#### 2022-05-05

站点主题从 Stack 更换为 Luna

#### 2021-11-14

小鸟拥有了自己的第一个私人博客

### 装修笔记索引

> [Stack 主题及评论区装修笔记](https://gregueria.icu/posts/decoration/)
>
> [Luna 主题装修笔记](https://gregueria.icu/posts/hugo-luna/)
>
> [📑 点击即看：上一版本的沙滩遗址](https://lastversion.vercel.app/)
