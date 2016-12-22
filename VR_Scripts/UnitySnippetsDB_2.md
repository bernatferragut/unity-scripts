---
layout: post
title: "VR - Intermediate Scripting in Unity"
description: "C# Snippet Compilation of Intermediate Unity scripting basics"
date: 2016-12-21
tags: [design, code, unity]
comments: true
share: true
---

## Intermediate Gameplay Scripting Guide in C#

> **01. Properties**

```C#
using UnityEngine;
using System.Collections;

public class Player : MonoBehaviour
{
    //Member variables can be referred to as fields.
    //By Getting or Setting you can make them visible or invisble
    public int Experience;
    {
        get
        {
            //Some other code
            return experience
        }
        set
        {
            //Some other code
            experience = value;
        }
    }

    //Level is property that converts experience
    //points into the level of a player automatically
    public int Level
    {
        get
        {
            return experience/1000;
        }
        set
        {
            experience = value * 1000;
        }
    }
    //This is an example of an autoimplemented property
    public int Health{ get; set;};
}

public class Game : MonoBehaviour
{
    void Start()
    {
        Player mPlayer = new Player();

        //Properties can be used just like variables
        mPlayer.Experience = 5;
        int x = mPlayer.Experience;
    }
}
```
> **02. TernaryOperator**

```C#
using UnityEngine;
using System.Collections;

public class TernaryOperator : MonoBehaviour
{
    void Start()
    {
        int health = 10;
        string message;

        //TernaryOperator choose message based on health
        //Similar to IF statements
        message = health>0 ?; "Players is alive" : "Playes is moonkied";
    }
}
```

> **03. Statics**

```C#
using UnityEngine;
using System.Collections;

public class Enemy
{
   //Static variables are shared across all instances of a class
   public static int enemmyCount = 0;

   public Enemy()
   {
       //Increment the static variable to know how many
       //objects of this class have been created
       enemmyCount++;
   }
}

public class 
{
   
}

public class 
{
   
}

public class 
{
   
}

public class 
{
   
}

public class 
{
   
}
```






