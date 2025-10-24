# Achieve-Cupertino-Style-in-MAUI-Switch

This sample demonstrates how to achieve a Cupertino-style appearance in the MAUI Switch within a .NET MAUI application.

## Sample

```xaml
    <ContentPage.Resources>
        <ResourceDictionary>
            <Style x:Key="CupertinoStyle" TargetType="buttons:SfSwitch">
                <Setter Property="VisualStateManager.VisualStateGroups">
                    <Setter.Value>
                        <VisualStateGroupList>
                            <VisualStateGroup x:Name="CommonStates">
                                <VisualState x:Name="On">
                                    <VisualState.Setters>
                                        <Setter Property="SwitchSettings">
                                            <Setter.Value>
                                                <buttons:SwitchSettings
                                                        ThumbBackground="White"
                                                        ThumbStroke="White"
                                                        ThumbHeightRequest="27"
                                                        ThumbWidthRequest="27"
                                                        TrackBackground="GreenYellow"
                                                        TrackStroke="LawnGreen"/>
                                            </Setter.Value>
                                        </Setter>
                                    </VisualState.Setters>
                                </VisualState>
                                <VisualState x:Name="Off">
                                    <VisualState.Setters>
                                        <Setter Property="SwitchSettings">
                                            <Setter.Value>
                                                <buttons:SwitchSettings
                                                        ThumbBackground="White"
                                                        ThumbStroke="White"
                                                        ThumbHeightRequest="27"
                                                        ThumbWidthRequest="27"
                                                        TrackBackground="Gray"
                                                        TrackStroke="DimGray"/>
                                            </Setter.Value>
                                        </Setter>
                                    </VisualState.Setters>
                                </VisualState>
                            </VisualStateGroup>
                        </VisualStateGroupList>
                    </Setter.Value>
                </Setter>
            </Style>
        </ResourceDictionary>
    </ContentPage.Resources>

    <VerticalStackLayout>

        <buttons:SfSwitch Style="{StaticResource CupertinoStyle}"/>

        <Label Text="Cupertino" FontSize="18" HorizontalOptions="Center"/>

    </VerticalStackLayout>
```

## Requirements to run the demo

To run the demo, refer to [System Requirements for .NET MAUI](https://help.syncfusion.com/maui/system-requirements)

## Troubleshooting:

### Path too long exception

If you are facing path too long exception when building this example project, close Visual Studio and rename the repository to short and build the project.

## License

Syncfusion has no liability for any damage or consequence that may arise from using or viewing the samples. The samples are for demonstrative purposes. If you choose to use or access the samples, you agree to not hold Syncfusion liable, in any form, for any damage related to use, for accessing, or viewing the samples. By accessing, viewing, or seeing the samples, you acknowledge and agree Syncfusion's samples will not allow you seek injunctive relief in any form for any claim related to the sample. If you do not agree to this, do not view, access, utilize, or otherwise do anything with Syncfusion's samples
