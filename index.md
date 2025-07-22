---
layout: default
title: Super Button for Unity
---

# 🎮 Super Button

A **free Unity plugin** that lets you add stylish and functional editor buttons to your `MonoBehaviour` scripts with ease.

![Super Button Banner](https://via.placeholder.com/1000x300?text=Super+Button+for+Unity)

---

## ✨ Features

- 🖱️ **One-click method execution** in the Inspector  
- 🎨 **Customizable colors, labels, icons, and tooltips**  
- 🧩 **Supports static, private, and parameterless methods**  
- 🛠️ **Lightweight and easy to integrate**  
- 🧑‍💻 Perfect for tools and rapid development

---

## 🧪 Example Usage

```csharp
using UnityEngine;

namespace SuperButton
{
    public class Test : MonoBehaviour
    {
        [SuperButton]
        public void Test1()
        {
            Debug.Log("Test1");
        }

        [SuperButton(">>>Test2<<<")]
        public void Test2()
        {
            Debug.Log("Test2");
        }

        [SuperButton(colorHex: "#D7D928")]
        private void Test3()
        {
            Debug.Log("Test3");
        }

        [SuperButton("Test4", buttonHeight: 20)]
        public void Test4()
        {
            Debug.Log("Test4");
        }

        [SuperButton(iconPath: "Assets/Super Button/Editor/Test.png")]
        public void Test5()
        {
            Debug.Log("Test5");
        }

        [SuperButton(tooltip: "This is a tooltip")]
        public void Test6()
        {
            Debug.Log("Test6");
        }

        [SuperButton(tooltip: "This is a static method")]
        public static void Test7()
        {
            Debug.Log("Test7");
        }
    }
}
