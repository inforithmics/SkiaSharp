# SkiaSharp

[![SkiaSharp](https://img.shields.io/nuget/vpre/SkiaSharp.svg?maxAge=2592000&label=SkiaSharp%20nuget)](https://www.nuget.org/packages/SkiaSharp)  [![SkiaSharp.Views](https://img.shields.io/nuget/vpre/SkiaSharp.Views.svg?maxAge=2592000&label=SkiaSharp.Views%20nuget)](https://www.nuget.org/packages/SkiaSharp.Views)  [![SkiaSharp.Views.Forms](https://img.shields.io/nuget/vpre/SkiaSharp.Views.Forms.svg?maxAge=2592000&label=SkiaSharp.Views.Forms%20nuget)](https://www.nuget.org/packages/SkiaSharp.Views.Forms)  
[![Gitter.im](https://img.shields.io/badge/gitter.im-xamarin%2FXamarinComponents-E60256.svg)](https://gitter.im/xamarin/XamarinComponents)  [![Xamarin Forums](https://img.shields.io/badge/forums-Graphics%20%26%20Games%2FSkiaSharp-1faece.svg)](https://forums.xamarin.com/categories/skiasharp)  
[![API Docs](https://img.shields.io/badge/docs-api-1faece.svg)](https://developer.xamarin.com/api/root/SkiaSharp/)  [![API Docs](https://img.shields.io/badge/docs-guides-1faece.svg)](https://docs.microsoft.com/en-us/xamarin/graphics-games/skiasharp/)  
[![Build Status](https://jenkins.mono-project.com/buildStatus/icon?job=SkiaSharp-Pipeline/master)](https://jenkins.mono-project.com/job/SkiaSharp-Pipeline/master)

SkiaSharp is a cross-platform 2D graphics API for .NET platforms based on Google's
Skia Graphics Library (https://skia.org/). It provides a comprehensive 2D API that can
be used across mobile, server and desktop models to render images.

SkiaSharp provides cross-platform bindings for:

 - .NET Standard 1.3
 - .NET Core
 - Tizen
 - Xamarin.Android
 - Xamarin.iOS
 - Xamarin.tvOS
 - Xamarin.watchOS
 - Xamarin.Mac
 - Windows Classic Desktop (Windows.Forms / WPF)
 - Windows UWP (Desktop / Mobile / Xbox / HoloLens)

The [API Documentation](https://developer.xamarin.com/api/namespace/SkiaSharp/) is
available on the web to browse.

## Using SkiaSharp

SkiaSharp is available as a convenience NuGet package, to use install the package like this:

```
nuget install SkiaSharp
```

_Because there are multiple distros of Linux, and we cannot possibly support them all, we have a separate NuGet package that will contain the supported binaries for a few distros: [SkiaSharp.NativeAssets.Linux](https://www.nuget.org/packages/SkiaSharp.NativeAssets.Linux). ([distros](https://github.com/mono/SkiaSharp/issues/453)) ([more info](https://github.com/mono/SkiaSharp/issues/312))_

## Building SkiaSharp

Before building SkiaSharp:

 * [Python 2.7](https://www.python.org/downloads) is available in the `PATH` environment variable on Windows
 * [Android NDK r14](https://developer.android.com/ndk/downloads/index.html) is available in the `ANDROID_NDK_HOME` environment variable on macOS
 * [.NET Core](https://www.microsoft.com/net/core) is installed on all platforms

First, clone the repository:

    $ git clone https://github.com/mono/SkiaSharp.git

Next, set up the submodules:

    $ cd SkiaSharp
    $ git submodule update --init --recursive

Finally, build everything:

Mac/Linux:

    $ ./bootstrapper.sh -t everything

Windows:

    > .\bootstrapper.ps1 -t everything

## Compare Code

Here are some links to show the differences in our code as compared to Google's code.

What version are we on? [**m68**](https://github.com/google/skia/tree/chrome/m68)  
Are we up-to-date with Google? [Compare](https://github.com/mono/skia/compare/xamarin-mobile-bindings...google:chrome/m68)  
What have we added? [Compare](https://github.com/google/skia/compare/chrome/m68...mono:xamarin-mobile-bindings)  
