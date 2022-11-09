### Paint Drying

## Paint Drying

**Project description:** A C# object orientated console application. My favorite demo from Programming 101.

### 1. Custom Classes

```javascript
Game.cs       
Program.cs
Player.cs
Menu.cs
ConsoleUtils.cs
CreditScene.cs
GarageScene.cs
Navigation.cs
RoomScene.cs
Scene.cs
TitleScene.cs

```

### 2. Conditional Statements

```javascript
 for (int i = 0; i < Options.Length; i++)
  { 
    string currentOption = Options[i];
    string prefix;
    if (i == SelectedIndex)
    {
      prefix = "*";
      ForegroundColor = ConsoleColor.Black;
      BackgroundColor = ConsoleColor.White;
    }
    else
    {
      prefix = " ";
      ForegroundColor = ConsoleColor.White;
      BackgroundColor = ConsoleColor.Black;
    }
    WriteLine($"{prefix} << {currentOption} >>");
    }
}
```

### 3. Collection of Data

```javascript
public void Run()
{
string prompt = $@"{RoomArt}
Well, heres your room. The wall is pretty boring. What do you want to do?";
string[] options = { "Go Someplace Else", "Look Under Desk", "Paint the Wall" };
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).
