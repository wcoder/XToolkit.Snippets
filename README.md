# XToolkit.Snippets

Snippets for Xamarin.Android and Xamarin.iOS.

## Importing snippets

### Visual Studio for Mac

You can import snippets by putting the files from the **VS4Mac** folder into `~/Library/VisualStudio/8.0/Snippets/`

### Rider

To import Snippets in Rider go to **Preferences > Manage Layers > Import from file**, select the **Live templates** checkbox and click OK. For more documentation see the [Rider documentation about Sharing Live Templates](https://www.jetbrains.com/help/rider/Sharing_Live_Templates.html).

## Snippets

### xprop

```cs
private string _name;
public string Name
{
    get => _name;
    private set => Set(ref _name, value);
}
```

### xcom

```cs
GoNextCommand = new RelayCommand(GoNext);

public ICommand GoNextCommand { get; }

private void GoNext()
{
}
```

### xcomt

```cs
FindCommand = new RelayCommand<string>(Find);

public ICommand<string> FindCommand { get; }

private void Find(string arg)
{
}
```

### xcoma

```cs
GoNextCommand = new AsyncCommand(GoNextAsync);

public IAsyncCommand GoNextCommand { get; }

private Task GoNextAsync()
{
}
```

### xcomat

```cs
FindCommand = new AsyncCommand<string>(FindAsync);

public IAsyncCommand<string> FindCommand { get; }

private Task FindAsync(string arg)
{
}
```

### xvm

```cs
public class HomePageViewModel : ViewModelBase
{
    public HomePageViewModel()
    {
    }

    public override void OnInitialize()
    {
        base.OnInitialize();
    }

    public override void OnAppearing()
    {
        base.OnAppearing();
    }

    public override void OnDisappearing()
    {
        base.OnDisappearing();
    }
}
```

### xbind

```cs
this.Bind(() => ViewModel.Title, () => TitleLabel.Text);
```

### xtest

```cs
[Fact]
public void UnitUnderTest_StateUnderTest_ExpectedResult()
{
}
```

---
&copy; 2020 | MIT
