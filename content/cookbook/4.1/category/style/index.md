---
title: "Style - ScottPlot 4.1 Cookbook"
description: "Plots can be styled to customize their colors and fonts."
date: 9/8/2022 9:21:28 PM
---

* This page contains recipes for the _Style_ category.
* Visit the [Cookbook Home Page](../../) to view all cookbook recipes.
* Generated by ScottPlot 4.1.58 on 9/8/2022
## Default Style

Customize many plot features using style presets

```cs
var plt = new ScottPlot.Plot(600, 400);

plt.AddSignal(DataGen.Sin(51));
plt.AddSignal(DataGen.Cos(51));

plt.Style(Style.Default);
plt.Title("Style.Default");
plt.XLabel("Horizontal Axis");
plt.YLabel("Vertical Axis");

plt.SaveFig("style_Default.png");
```

<img src='../../images/style_default.png' class='d-block mx-auto my-5' />


## Monospace Style

Customize many plot features using style presets

```cs
var plt = new ScottPlot.Plot(600, 400);

plt.AddSignal(DataGen.Sin(51));
plt.AddSignal(DataGen.Cos(51));

plt.Style(Style.Monospace);
plt.Title("Style.Monospace");
plt.XLabel("Horizontal Axis");
plt.YLabel("Vertical Axis");

plt.SaveFig("style_monospace.png");
```

<img src='../../images/style_monospace.png' class='d-block mx-auto my-5' />


## Blue1 Style

Customize many plot features using style presets

```cs
var plt = new ScottPlot.Plot(600, 400);

plt.AddSignal(DataGen.Sin(51));
plt.AddSignal(DataGen.Cos(51));

plt.Style(Style.Blue1);
plt.Title("Style.Blue1");
plt.XLabel("Horizontal Axis");
plt.YLabel("Vertical Axis");

plt.SaveFig("style_blue1.png");
```

<img src='../../images/style_blue1.png' class='d-block mx-auto my-5' />


## Blue2 Style

Customize many plot features using style presets

```cs
var plt = new ScottPlot.Plot(600, 400);

plt.AddSignal(DataGen.Sin(51));
plt.AddSignal(DataGen.Cos(51));

plt.Style(Style.Blue2);
plt.Title("Style.Blue2");
plt.XLabel("Horizontal Axis");
plt.YLabel("Vertical Axis");

plt.SaveFig("style_blue2.png");
```

<img src='../../images/style_blue2.png' class='d-block mx-auto my-5' />


## Light1 Style

Customize many plot features using style presets

```cs
var plt = new ScottPlot.Plot(600, 400);

plt.AddSignal(DataGen.Sin(51));
plt.AddSignal(DataGen.Cos(51));

plt.Style(Style.Light1);
plt.Title("Style.Light1");
plt.XLabel("Horizontal Axis");
plt.YLabel("Vertical Axis");

plt.SaveFig("style_light1.png");
```

<img src='../../images/style_light1.png' class='d-block mx-auto my-5' />


## Gray1 Style

Customize many plot features using style presets

```cs
var plt = new ScottPlot.Plot(600, 400);

plt.AddSignal(DataGen.Sin(51));
plt.AddSignal(DataGen.Cos(51));

plt.Style(Style.Gray1);
plt.Title("Style.Gray1");
plt.XLabel("Horizontal Axis");
plt.YLabel("Vertical Axis");

plt.SaveFig("style_Gray1.png");
```

<img src='../../images/style_gray1.png' class='d-block mx-auto my-5' />


## Black Style

Customize many plot features using style presets

```cs
var plt = new ScottPlot.Plot(600, 400);

plt.AddSignal(DataGen.Sin(51));
plt.AddSignal(DataGen.Cos(51));

plt.Style(Style.Black);
plt.Title("Style.Black");
plt.XLabel("Horizontal Axis");
plt.YLabel("Vertical Axis");

plt.SaveFig("style_Black.png");
```

<img src='../../images/style_black.png' class='d-block mx-auto my-5' />


## Seaborn Style

Customize many plot features using style presets

```cs
var plt = new ScottPlot.Plot(600, 400);

plt.AddSignal(DataGen.Sin(51));
plt.AddSignal(DataGen.Cos(51));

plt.Style(Style.Seaborn);
plt.Title("Style.Seaborn");
plt.XLabel("Horizontal Axis");
plt.YLabel("Vertical Axis");

plt.SaveFig("style_Seaborn.png");
```

<img src='../../images/style_seaborn.png' class='d-block mx-auto my-5' />


## Data Background Image

A backgorund image can be drawn behind the data area. Users to do this may want to make grid lines semitransparent.

```cs
var plt = new ScottPlot.Plot(600, 400);

plt.AddSignal(DataGen.Sin(51), 1, Color.Yellow);
plt.AddSignal(DataGen.Cos(51), 1, Color.Magenta);

Bitmap monaLisaBmp = ScottPlot.DataGen.SampleImage();

plt.Style(
    grid: Color.FromArgb(50, Color.White),
    dataBackgroundImage: monaLisaBmp);

plt.SaveFig("misc_background_image_data.png");
```

<img src='../../images/misc_background_image_data.png' class='d-block mx-auto my-5' />


## Figure Background Image

A backgorund image can be drawn behind the entire figure. If you do this you likely want to make your data background transparent.

```cs
var plt = new ScottPlot.Plot(600, 400);

plt.AddSignal(DataGen.Sin(51), 1, Color.Yellow);
plt.AddSignal(DataGen.Cos(51), 1, Color.Magenta);

Bitmap monaLisaBmp = ScottPlot.DataGen.SampleImage();

plt.Style(
    grid: Color.FromArgb(50, Color.White),
    tick: Color.White,
    dataBackground: Color.FromArgb(50, Color.White),
    figureBackgroundImage: monaLisaBmp);

plt.SaveFig("misc_background_image_figure.png");
```

<img src='../../images/misc_background_image_figure.png' class='d-block mx-auto my-5' />



