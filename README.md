# Maui XAML and Object Model Suggestions
This is a repo to hold suggestions for MAUI architecural and naming considerations as it is being developed. The origin and inspiration for this repository is formed from the discussion in https://github.com/dotnet/maui/issues/43.

> As a quick example, here is the comparison between a traditional XAML control for text `TextBlock` next to the Xamarin.Forms text control `Label`

| Platform | Hiearchy |
| -------- | -------- |
| UWP TextBlock | ![UWP TextBlock](https://user-images.githubusercontent.com/3520532/83947709-c3f2b000-a7e6-11ea-8a79-ed8a8509a890.png) |
| Xamarin.Forms Label | ![Xamarin.Forms Label](https://user-images.githubusercontent.com/3520532/83947730-de2c8e00-a7e6-11ea-8545-bb87136be6f2.png) |

## Contributing

Please add your suggesitons/fixes, pull request is super-easy and fast on GitHub

1. Click the little Pencil button at the top-right of this document
    * This will automatically fork the repo and you can start editing immediately.
2. Make your additions and open a Pull Request
    * The commit button at the bottom of the page will start a pull request for you.

## Suggestions

### General

| Xamarin.Forms XAML | Traditional XAML           | Proposal                                    |
|--------------------|----------------------------|---------------------------------------------|
| ContentPage        | Page                       | Page                                        |
| Object             | Object                     | Object                                      |
| BindableObject     | DependencyObject           | DependencyObject                            |
| BindableProperty   | DependencyProperty         | DependencyProperty                          |
| Element            | UIElement                  | UIElement                                   |
| NavigatableElement | ?                          | ?                                           |
| VisualElement      | FrameworkElement           | FrameworkElement                            |
| View               | ContentControl             | ContentControl                              |
| ContentView        | UserControl                | UserControl                                 |
| ContentPresenter   | ContentPresenter           | ContentPresenter                            |

### Controls

| Xamarin.Forms XAML | Traditional XAML           | Proposal                                    |
|--------------------|----------------------------|---------------------------------------------|
| Label              | TextBlock                  | TextBlock                                   |
| Entry              | TextBox                    | TextBox                                     |
| Editor             | RichTextBox                | RichTextBox                                 |
| Picker             | ComboBox                   | ComboBox                                    |
| StackLayout        | StackPanel                 | StackPanel                                  |
| ScrollView         | ScrollViewer               | ScrollViewer                                |
| Switch             | ToggleSwitch               | ToggleSwitch                                |
| Stepper            | NumericUpDown              | NumberBox                                   |
| Frame              | Border                     | Border                                      |
| Slider             | Slider                     | Slider                                      |
| ActivityIndicator  | ProgressRing               | ProgressRing                                |
| ?                  | ProgressBar                | ProgressBar                                 |
 
### Common Properties 
 
| Xamarin.Forms XAML | Traditional XAML           | Proposal                                    |
|------------------- |----------------------------|---------------------------------------------|
| HorizontalOptions  | HorizontalAlignment        | HorizontalAlignment                         |
| VerticalOptions    | VerticalAlignment          | VerticalAlignment                           |
| BindingContext     | DataContext                | DataContext                                 |
| BackgroundColor    | Background                 | Background                                  |
| TextColor          | Foreground                 | Foreground                                  |
| HeightRequest      | Height                     | Height                                      |
| WidthRequest       | Width                      | Width                                       |
| IsVisible          | Visibility                 | Visibility                                  |

### Object Model

Community Suggestions. Visit the origin to see full discussions around the idea.

| Suggestion | Origin                  |
| ---------- | ----------------------- |
| Base Architecture (fork from): UWP | [Pull Request #4](https://github.com/LanceMcCarthy/MauiSuggestions/pull/4) |
| XAML-defined animations (without attaching behaviors) | [Issue #1](https://github.com/LanceMcCarthy/MauiSuggestions/issues/1) |



