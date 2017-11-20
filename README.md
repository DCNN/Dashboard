# Distributed CNN Project

## 问题简述

由于移动端设备的计算能力、内存资源、电池续航等条件的限制，在需要执行深度神经网络时未免有些捉襟见肘，而直接推送任务到云端服务器进行解决也会由于其带来的延迟问题以及日益增长的数据流量而变得难以接受，这种时候我们思考是否可以将诸如此类的任务分担到附近的边缘设备（手机、PC、IOT设备）中进行解决。

## 项目目标

1. 设计分配具体任务给各个 slave 的算法；
1. 设计并实现一个 Android 端的 master APP(Group Owner)，作为任务的发起者；
1. 设计并实现具体 slave 执行任务的逻辑；
1. 考虑 slave 的异质性，并尝试使用 WebSocket 协议进行解决；

## 技术栈

1. Master 端暂定使用 Java 实现一个 WebSocket 服务器；
1. Slave 端使用 Vue 制作 UI，并通过 JavaScript 以及 Google 的 Deeplearning.js 完成 Master 分派的任务。
