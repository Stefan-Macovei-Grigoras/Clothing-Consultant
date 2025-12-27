# Clothing-Consultant
## What It Does

Gets weather info from Google for any location and suggests what to wear.

## How It Works

```
Main.xaml
├── Input.xaml - Ask user for location
├── OpenBrowser.xaml - Search on Google
├── GetData.xaml - Get temperature and conditions
└── Output.xaml - Show recommendations
```

## What You'll Learn

### Arguments
- **In** = data coming into the workflow
- **Out** = data going out of the workflow
- Names must match exactly (case-sensitive)

### VB.NET Basics
```vb
' Check if empty
If String.IsNullOrEmpty(variable) Then

' Check boolean
If pageSwitched Then

' String operations
variable.ToLower.Contains("rain")
String.Format("{0} degrees", temperature)

' Convert to number
CInt(temperature) < 15
```

### Best Practices Used

**Modular Design**
- Each workflow does one thing
- Easy to debug and reuse

**Error Handling**
- Validate user input
- Check if page loaded correctly
- Throw exceptions when something fails

**Browser Automation**
- Maximize window first
- Use Simulate mode for speed
- Verify elements exist
- Close browser when done

**Naming Conventions**
- `in_` for input arguments
- `out_` for output arguments
- Descriptive names

**Logging**
- Add log messages for tracking progress

## How to Run

1. Open in UiPath Studio
2. Run Main.xaml
3. Enter a city name
4. Bot shows weather and clothing advice

## Common Errors

**"Object reference not set"**
- Variable is null/empty
- Fix: Check variables are initialized

**"Element outside screen bounds"**
- Window too small or element hidden
- Fix: Maximize window or use Simulate mode

**"Argument does not map"**
- Argument name mismatch
- Fix: Check spelling and case in both workflows
