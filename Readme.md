# Xamarin.Forms.CustomSwitch [![Nuget](https://img.shields.io/nuget/v/IeuanWalker.CustomSwitch)](https://www.nuget.org/packages/IeuanWalker.CustomSwitch) [![Nuget](https://img.shields.io/nuget/dt/IeuanWalker.CustomSwitch)](https://www.nuget.org/packages/IeuanWalker.CustomSwitch) 

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2FIeuanWalker%2FXamarin.Forms.CustomSwitch.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2FIeuanWalker%2FXamarin.Forms.CustomSwitch?ref=badge_shield)

This is a switch/ toggle control that would alow you to create any style switch you'd like.
Taka a look at the sample app included within this project -

![Sample App](Doc/SampleApp.gif)

## How to use it?
Install the [NuGet package](https://www.nuget.org/packages/IeuanWalker.CustomSwitch) into your shared project project
```
Install-Package IeuanWalker.CustomSwitch
```

## What can I do with it?
### Properties
| Property | What it does | Extra info |
|---|---|---- |
| IsToggled | A `bool` to indicate the togles status of the switch | Default value is **false** |
| KnobHeight | The height of the knob on the switch | Default value is **0** |
| KnobWidth | The width of the knob on the switch | Default value is **0** |
| KnobColor | The solid color of the knob | Default value is **Color.Default** |
| KnobColorGradientStops | Sets the gradient colors for the Knob. <br> This is property exposed from [PancakeView](https://github.com/sthewissen/Xamarin.Forms.PancakeView)  | More info on how to use this in the [PancakeView docs](https://github.com/sthewissen/Xamarin.Forms.PancakeView/wiki/Gradients) <br> Default value is **new GradientStopCollection()** |
| KnobColorGradientStartPoint | Defines the relative start point of the gradient. <br> This is property exposed from [PancakeView](https://github.com/sthewissen/Xamarin.Forms.PancakeView)  | More info on how to use this in the [PancakeView docs - Gradients](https://github.com/sthewissen/Xamarin.Forms.PancakeView/wiki/Gradients) <br> Default value is **0,0** |
| KnobColorGradientEndPoint | Defines the relative endpoint of the gradient. <br> This is property exposed from [PancakeView](https://github.com/sthewissen/Xamarin.Forms.PancakeView)  | More info on how to use this in the [PancakeView docs - Gradients](https://github.com/sthewissen/Xamarin.Forms.PancakeView/wiki/Gradients) <br> Default value is **1,0** |
| KnobBorder | The border for the knob. <br> This is property exposed from [PancakeView](https://github.com/sthewissen/Xamarin.Forms.PancakeView)  | More info on how to use this in the [PancakeView docs - Borders](https://github.com/sthewissen/Xamarin.Forms.PancakeView/wiki/Borders) <br> Default value is **default(Border)** |
| KnobCornerRadius | A `CornerRadius` object representing each individual corner's radius for the knob. <br> This is property exposed from [PancakeView](https://github.com/sthewissen/Xamarin.Forms.PancakeView)  | More info on how to use this in the [PancakeView docs - Rounded corners](https://github.com/sthewissen/Xamarin.Forms.PancakeView/wiki/Rounded-Corners) <br> Default value is **default(CornerRadius)** |
| HeightRequest | The Height of the switch  | Default value is **0** |
| WidthRequest | The width of the switch  | Default value is **0** |
| CornerRadius | A `CornerRadius` object representing each individual corner's radius for the switch. <br> This is property exposed from [PancakeView](https://github.com/sthewissen/Xamarin.Forms.PancakeView)  | More info on how to use this in the [PancakeView docs - Rounded corners](https://github.com/sthewissen/Xamarin.Forms.PancakeView/wiki/Rounded-Corners) <br> Default value is **default(CornerRadius)** |
| BackgroundColor | The solid color of the switch | Default value is **Color.Default** |
| BackgroundColorGradientStops | Sets the gradient colors for the switch. <br> This is property exposed from [PancakeView](https://github.com/sthewissen/Xamarin.Forms.PancakeView)  | More info on how to use this in the [PancakeView docs](https://github.com/sthewissen/Xamarin.Forms.PancakeView/wiki/Gradients) <br> Default value is **new GradientStopCollection()** |
| BackgroundColorGradientStartPoint | Defines the relative start point of the gradient. <br> This is property exposed from [PancakeView](https://github.com/sthewissen/Xamarin.Forms.PancakeView)  | More info on how to use this in the [PancakeView docs - Gradients](https://github.com/sthewissen/Xamarin.Forms.PancakeView/wiki/Gradients) <br> Default value is **0,0** |
| BackgroundColorGradientEndPoint | Defines the relative endpoint of the gradient. <br> This is property exposed from [PancakeView](https://github.com/sthewissen/Xamarin.Forms.PancakeView)  | More info on how to use this in the [PancakeView docs - Gradients](https://github.com/sthewissen/Xamarin.Forms.PancakeView/wiki/Gradients) <br> Default value is **1,0** |
| Border | The border for the switch. <br> This is property exposed from [PancakeView](https://github.com/sthewissen/Xamarin.Forms.PancakeView)  | More info on how to use this in the [PancakeView docs - Borders](https://github.com/sthewissen/Xamarin.Forms.PancakeView/wiki/Borders) <br> Default value is **default(Border)** |
| BackgroundContent | Sets the content of the switch.  <br> See [samples](/Sample/Sample/Sample/Examples/) for an  idea how to utilise it  | Default value is **null** |
| KnobContent | Sets the content of the knob.  <br> See [samples](/Sample/Sample/Sample/Examples/) for an  idea how to utilise it | Default value is **null** |
| HorizontalKnobMargin | Adds a margin to the max distance the knob can travel | Default value is **0** |
| KnobLimit | Used to calculate the knob position.  <br> See [samples](/Sample/Sample/Sample/Examples/) for an  idea how to utilise it | Default value is **KnobLimitEnum.Boundary** |
| VibrateDuration | Used to set the duration of the vibration when the switch is toggles | Default value is **20** <br> To disble the vibrate set the value to `0` |
| ToggleAnimationDuration | Used to set the duration of the toggle animation | Default value is **100** <br> To disble the animation set the value to `0` |

### Events
| Event | What it does | Extra info |
|---|---|---- |
| Toggled | Triggered when the switch is toggled | Default value is **false** |
| SwitchPanUpdate | Triggered when the switch is toggled or dragged. Used to handle the transition of the switch from one side to the other. <br> See [samples](/Sample/Sample/Sample/Examples/) for an  idea how to utilise it | Default value is **false** |

## Examples
### iOS ([xaml](/Sample/Sample/Sample/Examples/IosSwitch.xaml) / [code behind](/Sample/Sample/Sample/Examples/IosSwitch.xaml.cs))
![iOS example](Doc/iOS.gif)

### Android ([xaml](/Sample/Sample/Sample/Examples/AndroidSwitch.xaml) / [code behind](/Sample/Sample/Sample/Examples/AndroidSwitch.xaml.cs))
![iOS example](Doc/Android.gif)

### Theme 1 ([xaml](/Sample/Sample/Sample/Examples/Theme1Switch.xaml) / [code behind](/Sample/Sample/Sample/Examples/Theme1Switch.xaml.cs))
![Theme 1 example](Doc/Theme1.gif)

### Theme 2 ([xaml](/Sample/Sample/Sample/Examples/Theme2Switch.xaml) / [code behind](/Sample/Sample/Sample/Examples/Theme2Switch.xaml.cs))
![Theme 2 example](Doc/Theme2.gif)

### Other 1 ([xaml](/Sample/Sample/Sample/Examples/Other1Switch.xaml) / [code behind](/Sample/Sample/Sample/Examples/Other1Switch.xaml.cs))
![Other 1 example](Doc/Other1.gif)

### Other 2 ([xaml](/Sample/Sample/Sample/Examples/Other2Switch.xaml) / [code behind](/Sample/Sample/Sample/Examples/Other2Switch.xaml.cs))
![Other 2 example](Doc/Other2.gif)

### Other 3 ([xaml](/Sample/Sample/Sample/Examples/Other3Switch.xaml) / [code behind](/Sample/Sample/Sample/Examples/Other3Switch.xaml.cs))
![Other 3 example](Doc/Other3.gif)

### Other 4 ([xaml](/Sample/Sample/Sample/Examples/Other4Switch.xaml) / [code behind](/Sample/Sample/Sample/Examples/Other4Switch.xaml.cs))
![Other 4 example](Doc/Other4.gif)

### Other 5 ([xaml](/Sample/Sample/Sample/Examples/Other5Switch.xaml) / [code behind](/Sample/Sample/Sample/Examples/Other5Switch.xaml.cs))
![Other 5 example](Doc/Other5.gif)

## License
[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2FIeuanWalker%2FXamarin.Forms.CustomSwitch.svg?type=large)](https://app.fossa.com/projects/git%2Bgithub.com%2FIeuanWalker%2FXamarin.Forms.CustomSwitch?ref=badge_large)