# hello-world
Just another repository
---
学习GitHub
---
* Git
* SVN
* 列表三
<br>
济南市
<br>

`高亮`
<br>
[百度](http://www.baidu.com)
![天猫](https://img.alicdn.com/tfs/TB1MaLKRXXXXXaWXFXXXXXXXXXX-480-260.png "天猫Logo")

### Unity编辑器Unity Editor基础
```C#
using System.Collections;
using System.Collections.Generic;
using UnityEngine;
using UnityEditor;
using UnityEngine.UI;
public enum MyEnum
{
    Option1,
    Option2,
    Option3

}
[RequireComponent(typeof(Rigidbody))]
[HelpURL("http://www.baidu.com")]
[AddComponentMenu("Custom")]
public class EditorLearn : MonoBehaviour
{
    void Start()
    {

    }

    [ContextMenu("Custom Button")]
    public void ConMenu()
    {
        Debug.Log("Custom menu.");
    }

    [ContextMenuItem("add TestName", "ContextMenuFunn2")]
    public string testName = "";

    private void ContextMenuFunn2()
    {
        testName = "你好！";
    }

    [SerializeField] private int var = 10;

    [Header("BaseInfo")] [Multiline(5)] public string name;

    [Range(0, 200)] public int age;

    [Space(5)] [Tooltip("用于设置性别")] public string sex;

    [ContextMenu("OutputInfo")]
    void OutputInfo()
    {
        print(name + " " + age);

    }

    public MyEnum mEnum;
}
```
