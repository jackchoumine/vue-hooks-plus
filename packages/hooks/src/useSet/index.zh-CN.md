---
map:
  # 映射到docs的路径
  path: /useSet
---

# useSet

管理 Set 类型状态的 Hook。

## 代码演示

<demo src="./demo/demo.vue"
  language="vue"
  title="基本用法"
  desc=""> </demo>

## API

```typescript
const [
  set,
  {
    add,
    remove,
    reset
  }
] = useSet(initialValue?: Iterable<K>);
```

## Result

| 参数   | 说明         | 类型                 |
| ------ | ------------ | -------------------- |
| set    | Set 对象     | `Ref<Set>`           |
| add    | 添加元素     | `(key: any) => void` |
| remove | 移除元素     | `(key: any) => void` |
| reset  | 重置为默认值 | `() => void`         |

## Params

| 参数         | 说明                        | 类型          | 默认值 |
| ------------ | --------------------------- | ------------- | ------ |
| initialValue | 可选项，传入默认的 Set 参数 | `Iterable<K>` | -      |
