---
title: Taro.startGyroscope(option)
sidebar_label: startGyroscope
---

开始监听陀螺仪数据。

> [参考文档](https://developers.weixin.qq.com/miniprogram/dev/api/device/gyroscope/wx.startGyroscope.html)

## 类型

```tsx
(option: Option) => Promise<CallbackResult>
```

## 参数

### Option

| 参数 | 类型 | 必填 | 说明 |
| --- | --- | :---: | --- |
| complete | `(res: CallbackResult) => void` | 否 | 接口调用结束的回调函数（调用成功、失败都会执行） |
| fail | `(res: CallbackResult) => void` | 否 | 接口调用失败的回调函数 |
| interval | "game" or "ui" or "normal" | 否 | 监听陀螺仪数据回调函数的执行频率 |
| success | `(res: CallbackResult) => void` | 否 | 接口调用成功的回调函数 |

### interval

监听陀螺仪数据回调函数的执行频率

| 参数 | 说明 |
| --- | --- |
| game | 适用于更新游戏的回调频率，在 20ms/次 左右 |
| ui | 适用于更新 UI 的回调频率，在 60ms/次 左右 |
| normal | 普通的回调频率，在 200ms/次 左右 |

## API 支持度

| API | 微信小程序 | H5 | React Native |
| :---: | :---: | :---: | :---: |
| Taro.startGyroscope | ✔️ |  |  |
