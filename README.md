# Unity-Minimum-Window-Size

Set minimum window size for Windows build in Unity

![](min-size-0.gif)

#Usage

```c#
int minWidth = 200;
int minHeight = 300;

MinimumWindowSize.Set(minWidth, minHeight);
```

Don't forget to **.Reset()** before quitting,
otherwise application will quit with exception
```c#
public class Example : MonoBehaviour {

    private void OnApplicationQuit(){
        MinimumWindowSize.Reset();
    }
}
``` 
