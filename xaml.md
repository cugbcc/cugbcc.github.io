# 开发笔记

---

## 使用 WindowChrome 自定义标题栏

```
<Window>
    <WindowChrome.WindowChrome>
        <WindowChrome UseAeroCaptionButtons="False" CaptionHeight="0"/>
    </WindowChrome.WindowChrome>
    <Grid Name="MainGrid">
        <!-- 窗口内容 -->
    </Grid>
</Window>
```

```UseAeroCaptionButtons``` 确保原生标题栏的系统按键点到没用

```CaptionHeight``` 确保自定义标题栏所有位置都能点到（即原生标题栏高度为0）

并且要在初始化窗口时添加如下代码

```
MainGrid.MaxWidth = SystemParameters.WorkArea.Width;
MainGrid.MaxHeight = SystemParameters.WorkArea.Height;
```

---
