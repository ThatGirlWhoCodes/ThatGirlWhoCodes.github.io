### Numeric Guessing Game

## Numeric Guessing Game

**Project description:** 

### 1. Custom Classes

```javascript
Game.cs
Program.cs
```

### 2. Conditional Statements

```javascript
if (Guess == Target)
{
  Console.WriteLine("We are one in the same! I was thinking of " + Target);
}
else
{
  Console.WriteLine("Oh darn... I was thinking of " + Target + " better luck next time!");
}
```

### 3. Randomization

```javascript
Guess = Convert.ToInt32(Console.ReadLine());
Target = RandomNumber.Next(10) + 1;
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).
