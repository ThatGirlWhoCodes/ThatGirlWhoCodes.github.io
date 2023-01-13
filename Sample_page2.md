### Detonation

## WPF/GUI Application

**Project description:** This game is set in a military space where you (the user) are the Sargent, and you are assigned a mission to locate a bomb. You play the protagonist, help by finding tools and exploring different significant cities in hopes of finding the bomb and deactivating it.  

### 1. Custom Classes

```javascript
City.cs
Game.cs
Item.cs
Player.cs
MainWindow.xaml
CityListPage.xaml
CityPage.xaml
Greeting.xaml
MyInventoryPage.xaml
ResultPage.xaml
```

### 2. Conditional Statements

```javascript
if (String.IsNullOrEmpty(PlayerNameTextBox.Text))
{
  MessageBox.Show("Please enter your name");
  canNavigateToCityPage = false;
}

if (MainWindow.myGame.CurrentPlayer.AvatarImage == "assets/generic.jpg")
{
  MessageBox.Show("Please pick an avatar");
  canNavigateToCityPage = false;
}
if (canNavigateToCityPage)
{
  MainWindow.myGame.CurrentPlayer.Name = PlayerNameTextBox.Text;
  Uri pageUri = new Uri("CityListPage.xaml", UriKind.Relative);
  NavigationService.Navigate(pageUri);
  ((MainWindow)Application.Current.MainWindow).UpdateStatus();
}
```

```javascript
foreach (Item item in MainWindow.myGame.CurrentPlayer.Inventory)
{
  if (item == city.ItemOne || item == city.ItemTwo)
  {
    numberOfItemsUserHaveFromThisCity++;
  }
}
label.Content = $"{city.Name} ({numberOfItemsUserHaveFromThisCity}/2)";

if (numberOfItemsUserHaveFromThisCity == 2)
{
  rectangle.Visibility = Visibility.Visible;
}
else
{
  rectangle.Visibility = Visibility.Hidden;
}
```

### 3. Collection of Data

<img src="DetonationHomePage.png?raw=true"/>


For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).
