---
title: 模型"小窗"
--- 

## **ModelViewPlugin**

模型"小窗"将 **Five** 的**空间总览模态** `Five.Mode.Floorplan` 以"小窗"的形式渲染至某个 DOM 节点中，可达到全景与模型共存的状态。

## 示例效果

<div className="docs-vr-normal">
  <iframe className="docs-vr-iframe" src="https://realsee.js.org/dnalogelExamples/ModelviewPluginExample/"></iframe>
</div>

## 安装引用

```tsx
import ModelViewPlugin from "@realsee/dnalogel/plugins/floorplan/ModelViewPlugin"
```

## 开发指南

### 初始化

> 方法1：在初始化 `Five` 实例时，将 `ModelViewPlugin` 配置在初始化插件参数即可。

```ts
import { Five } from '@realsee/five'
import { ModelViewPlugin } from "@realsee/dnalogel";

const five = new Five({
    plugins: [
        [
            ModelViewPlugin,
            'modelView', // 自定义插件名称
            {
                // 参数配置
            }
        ]
    ]
})
```

> 方法2：在创建 `FiveProvider` 时，将 `TopviewFloorplanPlugin` 配置在初始化插件参数即可。

```ts
import { ModelViewPlugin } from "@realsee/dnalogel";
import { createFiveProvider, FiveCanvas } from "@realsee/five/react";

const FiveProvider = createFiveProvider({
    plugins: [
        [
            ModelViewPlugin,
            'modelView', // 自定义插件名称
            {
                // 参数配置
            }
        ]
    ]
});
```

### 节点挂载

通过`five.plugins.ModelView`方式获取 `ModelViewPlugin` 实例的引用。该插件实例提供两个方法：

- `appendTo(element: HTMLElement, size?: { width?: number; height?: number }): void`: 将渲染内容挂载至相关 `DOM` 节点
- `refresh(size?: { width?: number; height?: number }): void` : 强制刷新，即重新渲染一次。

通过 `appendTo` 方法将挂载 DOM 节点

```ts
five.plugins.modelView.appendTo(wrapperElement)

// refresh 方法使用示例
// five.plugins.modelView.refresh({ width: 160, height: 180 })
```

