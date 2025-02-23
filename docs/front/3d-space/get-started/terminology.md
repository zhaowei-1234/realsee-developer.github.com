---
title: 名词解释
---

## 什么是 **Work**

**Work** 是[如视开发者中心](https://developers.realsee.com) 提供的对于一个三维空间的描述。
是通过如视硬件设备（[如视扫描仪](https://realsee.com/website/product/hardware) 、[如视 **Lite** 全景相机](https://realsee.com/website/product/lite) 、[如视VR App](https://realsee.com/website/mobile) ）扫描并处理之后用于三维空间展示的数据。

**Work** 以 `JSON` 作为数据格式 **Five** 框架可以解析 **Work** 数据并展示。一个 **Five** 实例每次可以载入并展示一个 **Work** 。并且也可以在不同的 **Work** 之间动态切换。

**Work** 的数据样例如下

<details>
  <summary>点击查看 Work 数据示例</summary>

```json
{
  "initial": {
    "mode": "Panorama",
    "pano_index": 6,
    "longitude": 2.6869287662553916,
    "latitude": 0,
    "fov": 95
  },
  "model": {
    "file_url": "https:\/\/vrlab-public.ljcdn.com\/release\/auto3dhd\/a62e1ebf7d013f7df117551a14af79fc\/model\/auto3d-DJaa08PIzN4JYluXQ1j2VS.at3d",
    "material_textures": [
      "https:\/\/vrlab-public.ljcdn.com\/release\/auto3dhd\/a62e1ebf7d013f7df117551a14af79fc\/materials\/texture_0.jpg",
      "https:\/\/vrlab-public.ljcdn.com\/release\/auto3dhd\/a62e1ebf7d013f7df117551a14af79fc\/materials\/texture_1.jpg",
      "https:\/\/vrlab-public.ljcdn.com\/release\/auto3dhd\/a62e1ebf7d013f7df117551a14af79fc\/materials\/texture_2.jpg",
      "https:\/\/vrlab-public.ljcdn.com\/release\/auto3dhd\/a62e1ebf7d013f7df117551a14af79fc\/materials\/texture_3.jpg",
      "https:\/\/vrlab-public.ljcdn.com\/release\/auto3dhd\/a62e1ebf7d013f7df117551a14af79fc\/materials\/texture_4.jpg",
      "https:\/\/vrlab-public.ljcdn.com\/release\/auto3dhd\/a62e1ebf7d013f7df117551a14af79fc\/materials\/texture_5.jpg",
      "https:\/\/vrlab-public.ljcdn.com\/release\/auto3dhd\/a62e1ebf7d013f7df117551a14af79fc\/materials\/texture_6.jpg",
      "https:\/\/vrlab-public.ljcdn.com\/release\/auto3dhd\/a62e1ebf7d013f7df117551a14af79fc\/materials\/texture_7.jpg",
      "https:\/\/vrlab-public.ljcdn.com\/release\/auto3dhd\/a62e1ebf7d013f7df117551a14af79fc\/materials\/texture_8.jpg",
      "https:\/\/vrlab-public.ljcdn.com\/release\/auto3dhd\/a62e1ebf7d013f7df117551a14af79fc\/materials\/texture_9.jpg"
    ]
  },
  "panorama": {
    "list": [
      {
        "up": "https:\/\/vrlab-public.ljcdn.com\/release\/auto3dhd\/a62e1ebf7d013f7df117551a14af79fc\/images\/cube_2048\/0\/2257f0f0b29d5b00ff01934ce51aaa35\/0_u.jpg",
        "down": "https:\/\/vrlab-public.ljcdn.com\/release\/auto3dhd\/a62e1ebf7d013f7df117551a14af79fc\/images\/cube_2048\/0\/2257f0f0b29d5b00ff01934ce51aaa35\/0_d.jpg",
        "left": "https:\/\/vrlab-public.ljcdn.com\/release\/auto3dhd\/a62e1ebf7d013f7df117551a14af79fc\/images\/cube_2048\/0\/2257f0f0b29d5b00ff01934ce51aaa35\/0_l.jpg",
        "right": "https:\/\/vrlab-public.ljcdn.com\/release\/auto3dhd\/a62e1ebf7d013f7df117551a14af79fc\/images\/cube_2048\/0\/2257f0f0b29d5b00ff01934ce51aaa35\/0_r.jpg",
        "front": "https:\/\/vrlab-public.ljcdn.com\/release\/auto3dhd\/a62e1ebf7d013f7df117551a14af79fc\/images\/cube_2048\/0\/2257f0f0b29d5b00ff01934ce51aaa35\/0_f.jpg",
        "back": "https:\/\/vrlab-public.ljcdn.com\/release\/auto3dhd\/a62e1ebf7d013f7df117551a14af79fc\/images\/cube_2048\/0\/2257f0f0b29d5b00ff01934ce51aaa35\/0_b.jpg"
      },
      {
        "up": "https:\/\/vrlab-public.ljcdn.com\/release\/auto3dhd\/a62e1ebf7d013f7df117551a14af79fc\/images\/cube_2048\/1\/ecb554bb1c122fa90186d176ccfecde4\/1_u.jpg",
        "down": "https:\/\/vrlab-public.ljcdn.com\/release\/auto3dhd\/a62e1ebf7d013f7df117551a14af79fc\/images\/cube_2048\/1\/ecb554bb1c122fa90186d176ccfecde4\/1_d.jpg",
        "left": "https:\/\/vrlab-public.ljcdn.com\/release\/auto3dhd\/a62e1ebf7d013f7df117551a14af79fc\/images\/cube_2048\/1\/ecb554bb1c122fa90186d176ccfecde4\/1_l.jpg",
        "right": "https:\/\/vrlab-public.ljcdn.com\/release\/auto3dhd\/a62e1ebf7d013f7df117551a14af79fc\/images\/cube_2048\/1\/ecb554bb1c122fa90186d176ccfecde4\/1_r.jpg",
        "front": "https:\/\/vrlab-public.ljcdn.com\/release\/auto3dhd\/a62e1ebf7d013f7df117551a14af79fc\/images\/cube_2048\/1\/ecb554bb1c122fa90186d176ccfecde4\/1_f.jpg",
        "back": "https:\/\/vrlab-public.ljcdn.com\/release\/auto3dhd\/a62e1ebf7d013f7df117551a14af79fc\/images\/cube_2048\/1\/ecb554bb1c122fa90186d176ccfecde4\/1_b.jpg"
      }
    ],
  },
  "observers": [
    {
      "visible_nodes": [ 1 ],
      "accessible_nodes": [ 1 ],
      "quaternion": {
        "w": 0.45076583925142194,
        "x": 0.010070951976936936,
        "y": -0.8925839597148215,
        "z": -0.0016154299986102319
      },
      "standing_position": [
        -6.956049919128418,
        -1.3924440682333898,
        1.6591600179672241
      ],
      "position": [
        -6.956049919128418,
        -0.10312400013208389,
        1.6591600179672241
      ],
      "floor_index": 0
    },
    {
      "visible_nodes": [ 0 ],
      "accessible_nodes": [ 0 ],
      "index": 1,
      "quaternion": {
        "w": -0.9884643083591809,
        "x": -0.0038900979633806664,
        "y": 0.1512670435365699,
        "z": -0.006439990839033269
      },
      "standing_position": [
        -6.176340103149414,
        -1.380554749576384,
        2.179759979248047
      ],
      "position": [
        -6.176340103149414,
        -0.10025200247764587,
        2.179759979248047
      ],
      "floor_index": 0,
    }
  ]
}
```

</details>

Work 的数据说明

- `initial`: 初始化数据，是一个 `State` 数据。描述 **Work** 被加载初始状态的位姿，也叫做 VR 的初始视角
    - mode: 模态
    - pano_index: 初始化点位
    - longitude: 相机的水平角
    - latitude: 相机的偏航角
    - fov: 相机垂直方向的可视角度

- `model`: 三维模型
    - file_url: 三维模型的资源地址，文件为 `.at3d` 为如视定制的模型格式
    - material_textures: 三维模型的贴图资源地址

- `panorama`: 全景彩色信息
    - list:
        - up / down / left / right / front / back: 全景彩色信息以 [cubemap](https://en.wikipedia.org/wiki/Cube_mapping) 方式存储和使用。

- `observers`: 采集点信息
    - visible_nodes: 采集点之间的可见性列表
    - accessible_nodes: 采集点之间的连通性列表
    - quaternion: 采集点与模型坐标的旋转偏移量
    - standing_position: 采集点地面坐标
    - position: 采集点坐标
    - floor_index: 采集点楼层

## 什么是 Five State

**State** 是 **Five** 框架用于描述状态的数据结构。他包含了模态、位于的采集点位、相机的方向、相机可视角度的信息。
您可以使用 **State** 来操作 **Five** 或者获取 **Five** 当前的状态。

```ts
interface State {
  "mode": Five.Mode,
  "panoIndex": number,
  "longitude": number,
  "latitude": number,
  "fov": number,
}
```

**State**的数据描述

- `mode`: 当前的模态
  Five 常用有 5 种模态，可以使用 `Five.Mode` 获得
    - **Panorama: 全景游走模态**，该模态下视图将在采集点间游走，手势操作可以旋转/放大视角/切换采集点，适合查看采集的全景信息。
    - **Floorplan: 空间总览模态**, 该模态下视图以模型为中心，手势操作可以旋转/放大模型/切换楼层，适合查看模型的整体效果。
    - **Topview: 户型图模态**，该模态下视图以模型为中心，垂直俯视模型，手势操作可以平移/放大模型/切换楼层，适合查看模型平面结构。
    - **Model: 模型游走模态**，该模态下视图将在模型中自由游走，手势操作可以旋转/放大视角/位移，适合查看模型的细节，做一些定位操作。
    - **VRPanorama: VR 眼镜模态**，该模态下可以使用 [Cardboard 眼镜](https://arvr.google.com/cardboard/) 或者他的第三方衍生产品，实现 VR 虚拟显示效果。

- `panoIndex`: 采集点位

- `longitude` / `latitude`: 相机的水平角 / 相机的偏航角（弧度），我们使用类似经纬度的方式描述相机位置。

- `fov`: 相机垂直方向的可视角度 (角度)


