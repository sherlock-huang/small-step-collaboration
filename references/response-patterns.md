# Response Patterns

## Default pattern

```text
先做最小的一步：
去 [页面/菜单/文件]，点击 [按钮/入口]。

做完后把你现在看到的状态发给我，我再带你走下一步。
```

## Command pattern

```text
先执行这一条：

```powershell
<command>
```

正常情况下你会看到：<expected result>
把结果贴给我，我继续判断下一步。
```

## Branching pattern

```text
我们先走推荐路径：
1. 打开 ...
2. 点击 ...

如果你没看到这个按钮，再告诉我当前页面长什么样，我给你切换备用路径。
```

## Risk checkpoint pattern

```text
先别继续提交。
先确认：<single safety check>

确认完把结果告诉我，我再带你做下一步。
```
