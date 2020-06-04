# Maui XAML and Object Model Suggestions
This is a repo to hold suggestions for MAUI architecural and naming considerations as it is being developed.

Please add your ideas and suggesitons, pull request is super-easy and fast on GitHub

1. Click the little Pencil button at the top-right of this document
    * This will automatically fork the repo and you can start editing immediately.
2. Make your additions and open a Pull Request
    * The commit button at the bottom of the page will start a pull request for you.


Base Architecture (fork from): UWP

## Names

| Xamarin.Forms     | Other XAML                 | Proposal                                    |
|-------------------|----------------------------|---------------------------------------------|
| ContentPage       | Page                       | Page                                        |
| ContentView       | UserControl                |                                             |
| BindableProperty  | DependencyProperty         | DependencyProperty                          |
| BindableObject    | DependencyObject           | DependencyObject                            |
| VisualElement     | UIElement                  | UIElement                                   |
| View              | FrameworkElement           | FrameworkElement                            |
| ContentPresenter  | ContentPresenter           | ContentPresenter                            |
| ContentView       | ContentControl/UserControl | ContentControl/UserControl                  |
| Label             | TextBlock                  | TextBlock                                   |
| Entry             | TextBox                    | TextBox                                     |
| Editor            | RichTextBox                | RichTextBox                                 |
| Picker            | ComboBox                   | ComboBox                                    |
| StackLayout       | StackPanel                 | StackPanel                                  |
| ScrollView        | ScrollViewer               | ScrollViewer                                |
| Switch            | ToggleSwitch               | ToggleSwitch                                |
| Stepper           | NumericUpDown              | NumericStepper, NumericUpDown, NumericInput |
| Frame           | Border                     | Border                                      |
| Slider            | Slider                     | Slider                                      |
| ActivityIndicator | ProgressRing               | ProgressRing                                |

## Other
| Xamarin.Forms     | Other XAML                 | Proposal                                    |
|-------------------|----------------------------|---------------------------------------------|
| HorizontalOptions | HorizontalAlignment        | HorizontalAlignment                         |
| VerticalOptions   | VerticalAlignment          | VerticalAlignment                           |
| BindingContext    | DataContext                | DataContext                                 |
| BackgroundColor   | Background                 | Background                                  |
| TextColor         | Foreground                 | Foreground                                  |
| HeightRequest     | Height                     | Height                                      |
| WidthRequest      | Width                      | Width                                       |
| IsVisible         | Visibility                 | Visibility                                  |
