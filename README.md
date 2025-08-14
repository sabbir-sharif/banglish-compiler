# 🚀 Banglish Compiler

A unique programming language that combines **Bengali** and **English** keywords, making programming more accessible and intuitive for Bengali speakers.

## 📋 Table of Contents

- [Features](#-features)
- [Getting Started](#-getting-started)
- [Language Syntax](#-language-syntax)
- [Examples](#-examples)
- [Advanced Features](#-advanced-features)
- [Troubleshooting](#-troubleshooting)
- [Contributing](#-contributing)

## ✨ Features

- **Bengali-English Mix**: Use Bengali keywords like `dhori`, `dekhao`, `jodi`, `tahole`, `nahole`
- **Real-time Compilation**: Instant feedback with syntax highlighting
- **Arithmetic Operations**: Full support for `+`, `-`, `*`, `/`, `%` with proper precedence
- **Conditional Logic**: Nested if-else statements with complex conditions
- **Variable Management**: Dynamic variable declaration and assignment
- **Error Handling**: Clear error messages with debugging information
- **Responsive Design**: Works on desktop, tablet, and mobile devices

## 🚀 Getting Started

### Installation

1. **Download**: Save the `Mini_compiler.html` file to your computer
2. **Open**: Double-click the file or open it in any modern web browser
3. **Start Coding**: The compiler is ready to use immediately!

### System Requirements

- Any modern web browser (Chrome, Firefox, Safari, Edge)
- No additional software or plugins required
- Works offline - no internet connection needed

## 📖 Language Syntax

### Variables

```banglish
// Variable declaration
dhori variable_name = value

// Examples
dhori x = 10
dhori name = "John"
dhori result = 5 + 3
```

### Print Statements

```banglish
// Print variables or values
dekhao variable_name
dekhao "Hello World"
dekhao 42
```

### Arithmetic Operations

```banglish
dhori a = 10
dhori b = 5

dhori sum = a + b        // Addition: 15
dhori diff = a - b       // Subtraction: 5
dhori product = a * b    // Multiplication: 50
dhori quotient = a / b   // Division: 2
dhori remainder = a % b  // Modulo: 0
```

### Conditional Statements

```banglish
// Basic if-else
jodi (condition) tahole {
    // statements when true
} nahole {
    // statements when false
}

// Example
jodi (x > 5) tahole {
    dekhao "x is greater than 5"
} nahole {
    dekhao "x is 5 or less"
}
```

### Comparison Operators

| Operator | Meaning |
|----------|---------|
| `==` | Equal to |
| `!=` | Not equal to |
| `<` | Less than |
| `>` | Greater than |
| `<=` | Less than or equal |
| `>=` | Greater than or equal |

### Comments

```banglish
// This is a single-line comment
dhori x = 5  // Comments can be at the end of lines
```

## 🎯 Examples

### Example 1: Basic Calculator

```banglish
// Simple calculator
dhori num1 = 25
dhori num2 = 8

dhori sum = num1 + num2
dhori difference = num1 - num2
dhori product = num1 * num2
dhori quotient = num1 / num2

dekhao "Sum:"
dekhao sum
dekhao "Difference:"
dekhao difference
dekhao "Product:"
dekhao product
dekhao "Quotient:"
dekhao quotient
```


### Example 2: Temperature Converter

```banglish
// Celsius to Fahrenheit converter
dhori celsius = 25
dhori fahrenheit = celsius * 9 / 5 + 32

dekhao "Temperature in Celsius:"
dekhao celsius
dekhao "Temperature in Fahrenheit:"
dekhao fahrenheit

jodi (celsius > 30) tahole {
    dekhao "Hot weather!"
} nahole {
    dekhao "Pleasant weather"
}
```

### Example 3: Shopping Bill Calculator

```banglish
// Shopping bill with discount and tax
dhori item1 = 150
dhori item2 = 75
dhori item3 = 200

dhori subtotal = item1 + item2 + item3
dhori discount = subtotal * 10 / 100
dhori discounted_amount = subtotal - discount
dhori tax = discounted_amount * 5 / 100
dhori final_total = discounted_amount + tax

dekhao "Shopping Bill:"
dekhao "Subtotal:"
dekhao subtotal
dekhao "Discount (10%):"
dekhao discount
dekhao "After discount:"
dekhao discounted_amount
dekhao "Tax (5%):"
dekhao tax
dekhao "Final Total:"
dekhao final_total

jodi (final_total > 300) tahole {
    dekhao "Expensive shopping!"
} nahole {
    dekhao "Reasonable purchase"
}
```

### Example 4: Age Category Checker

```banglish
// Age category with multiple conditions
dhori birth_year = 2000
dhori current_year = 2024
dhori age = current_year - birth_year

dekhao "Your age:"
dekhao age

jodi (age < 13) tahole {
    dekhao "You are a child"
} nahole {
    dekhao "You are a teenager"
}
```





### Example 5: BMI Calculator

```banglish
// BMI Calculator with health recommendations
dhori weight_kg = 70
dhori height_cm = 175

// Convert height to meters and calculate BMI
dhori height_m = height_cm / 100
dhori bmi = weight_kg / (height_m * height_m)

dekhao "BMI Calculator Results:"
dekhao "Weight (kg):"
dekhao weight_kg
dekhao "Height (cm):"
dekhao height_cm
dekhao "BMI:"
dekhao bmi

// BMI Categories
jodi (bmi < 18.5) tahole {
    dekhao "Category: Underweight"
    dekhao "Recommendation: Consider gaining healthy weight"
} nahole {
    
        dekhao "Category: Normal weight"
        dekhao "Recommendation: Maintain current weight"
}

// Calculate ideal weight range (for height)
dhori ideal_weight_min = 18.5 * height_m * height_m
dhori ideal_weight_max = 24.9 * height_m * height_m

dekhao "Ideal weight range:"
dekhao ideal_weight_min
dekhao "to"
dekhao ideal_weight_max
```

### Complex Arithmetic

```banglish
// Operator precedence follows mathematical rules
dhori result = 2 + 3 * 4 - 1    // Result: 13 (not 19)
dhori complex = (5 + 3) * 2 / 4  // Result: 4

// Negative numbers
dhori negative = -10
dhori calculation = 5 - 15       // Result: -10
```

### Variable Reassignment

```banglish
dhori x = 10
dekhao x          // Prints: 10

x = 20            // Reassign without 'dhori'
dekhao x          // Prints: 20

x = x + 5         // Use variable in its own assignment
dekhao x          // Prints: 25
```

## 🐛 Troubleshooting

### Common Errors

#### 1. **Syntax Errors**
```banglish
❌ dhori x 5           // Missing '='
✅ dhori x = 5

❌ jodi x > 5 tahole   // Missing parentheses
✅ jodi (x > 5) tahole { }
```

#### 2. **Undefined Variables**
```banglish
❌ dekhao y           // Variable 'y' not declared
✅ dhori y = 10
   dekhao y
```

#### 3. **Division by Zero**
```banglish
❌ dhori result = 10 / 0
✅ dhori divisor = 5
   dhori result = 10 / divisor
```

#### 4. **Mismatched Braces**
```banglish
❌ jodi (x > 5) tahole {
     dekhao "greater"
   // Missing closing brace

✅ jodi (x > 5) tahole {
     dekhao "greater"
   }
```

### Tips for Success

1. **Always use parentheses** around conditions in `jodi` statements
2. **Match opening and closing braces** `{` and `}`
3. **Declare variables** with `dhori` before using them
4. **Use quotes** for string literals: `"text"` or `'text'`
5. **Check operator precedence** - use parentheses when in doubt

## 🎮 Interactive Features

### Control Buttons

- **🚀 Run Code**: Execute your Banglish program
- **🗑️ Clear**: Clear the editor and start fresh
- **📖 Load Example**: Load a sample program to get started

### Live Output

- See compilation results in real-time
- Clear error messages for debugging
- No variable clutter - only your program output

## 🌟 Best Practices

### 1. Code Organization
```banglish
// Use comments to explain your code
// Group related operations together

// Variable declarations
dhori width = 10
dhori height = 5

// Calculations
dhori area = width * height
dhori perimeter = 2 * (width + height)

// Output
dekhao "Area:"
dekhao area
dekhao "Perimeter:"
dekhao perimeter
```

### 2. Meaningful Variable Names
```banglish
// ✅ Good
dhori student_marks = 85
dhori total_students = 30

// ❌ Avoid
dhori x = 85
dhori y = 30
```

### 3. Use Nested Conditions Wisely
```banglish
// Break complex logic into smaller, readable parts
jodi (marks >= 60) tahole {
    jodi (marks >= 80) tahole {
        dekhao "Excellent!"
    } nahole {
        dekhao "Good job!"
    }
} nahole {
    dekhao "Need improvement"
}
```

## 🤝 Contributing

We welcome contributions to improve the Banglish Compiler! Here are ways you can help:

- **Report bugs** or suggest new features
- **Improve documentation** or add more examples
- **Enhance the compiler** with new language features
- **Create tutorials** or learning materials

## 📄 License

This project is open source and available under the MIT License.

## 🔗 Keywords Reference

| Bengali | English | Purpose |
|---------|---------|---------|
| `dhori` | declare/hold | Variable declaration |
| `dekhao` | show/print | Output statements |
| `jodi` | if | Conditional statement |
| `tahole` | then | If-block start |
| `nahole` | else | Else-block start |

---

## 🔧 Future Work

### Nested If-Else Statements
### Loop
### Array

**Happy Coding with Banglish! 🎉**

*Made with ❤️ *
