# C# Note

---

#### 使用 WindowChrome 自定义标题栏

```
<Window>
  <WindowChrome.WindowChrome>
    <WindowChrome UseAeroCaptionButtons="False" CaptionHeight="0"/>
  </WindowChrome.WindowChrome>
  <Grid>
  </Grid>
</Window>
```
```UseAeroCaptionButtons``` 确保原生标题栏的系统按键点到没用

```CaptionHeight``` 确保自定义标题栏所有位置都能点到（即原生标题栏高度为0）

---
