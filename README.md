# Meteora

Meteora is a dark, "don't-call-it-metro"-esque theme based on the 
[ExpressionDark](http://wpf.codeplex.com/wikipage?title=WPF%20Themes) theme.

To use the theme, put the following in the resource dictionary in your 
application resources (`App.xaml`):

```xml
<ResourceDictionary Source="/Meteora.WPF;component/Meteora.xaml" />
```

Your final `App.xaml` may look something like this:

```xml
<Application x:Class="MyAwesomeApp.App"
             xmlns="http://schemas.microsoft.com/winfx/2006/xaml/presentation"
             xmlns:x="http://schemas.microsoft.com/winfx/2006/xaml"
             xmlns:local="clr-namespace:MyAwesomeApp">
    <Application.Resources>
        <ResourceDictionary>
            <ResourceDictionary.MergedDictionaries>
                <ResourceDictionary Source="/Meteora.WPF;component/Meteora.xaml" />
                <ResourceDictionary>
                    <local:NinjectBootstrapper x:Key="bootstrapper" />
                </ResourceDictionary>
            </ResourceDictionary.MergedDictionaries>
        </ResourceDictionary>
    </Application.Resources>

</Application>
```