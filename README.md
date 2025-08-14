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

### Example 2: Grade Calculator

```banglish
// Grade calculator with nested conditions
dhori math = 85
dhori science = 92
dhori english = 78

dhori total = math + science + english
dhori average = total / 3

dekhao "Average marks:"
dekhao average

jodi (average >= 90) tahole {
    dekhao "Grade: A+"
} nahole {
    jodi (average >= 80) tahole {
        dekhao "Grade: A"
    } nahole {
        jodi (average >= 70) tahole {
            dekhao "Grade: B"
        } nahole {
            dekhao "Grade: C"
        }
    }
}
```

### Example 3: Temperature Converter

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
    jodi (celsius > 15) tahole {
        dekhao "Pleasant weather"
    } nahole {
        dekhao "Cold weather!"
    }
}
```

### Example 4: Shopping Bill Calculator

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

### Example 5: Age Category Checker

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
    jodi (age < 20) tahole {
        dekhao "You are a teenager"
        jodi (age >= 18) tahole {
            dekhao "You can vote!"
        } nahole {
            dekhao "Too young to vote"
        }
    } nahole {
        jodi (age < 60) tahole {
            dekhao "You are an adult"
            dhori retirement_years = 60 - age
            dekhao "Years to retirement:"
            dekhao retirement_years
        } nahole {
            dekhao "You are a senior citizen"
        }
    }
}
```

### Example 6: Number Analysis

```banglish
// Comprehensive number analysis
dhori number = -15

dekhao "Analyzing number:"
dekhao number

// Check positive/negative/zero
jodi (number > 0) tahole {
    dekhao "Number is positive"
    
    // Check even/odd for positive numbers
    dhori remainder = number % 2
    jodi (remainder == 0) tahole {
        dekhao "Number is even"
    } nahole {
        dekhao "Number is odd"
    }
    
    // Check if it's a perfect square
    dhori sqrt_approx = number / 2
    dhori square_check = sqrt_approx * sqrt_approx
    jodi (square_check == number) tahole {
        dekhao "Might be a perfect square"
    }
    
} nahole {
    jodi (number < 0) tahole {
        dekhao "Number is negative"
        dhori absolute_value = number * -1
        dekhao "Absolute value:"
        dekhao absolute_value
    } nahole {
        dekhao "Number is zero"
    }
}
```

### Example 7: Loan Interest Calculator

```banglish
// Loan calculator with different interest rates
dhori principal = 100000
dhori years = 5

dekhao "Loan Calculator"
dekhao "Principal amount:"
dekhao principal
dekhao "Loan period (years):"
dekhao years

// Different rates based on loan amount
dhori interest_rate = 0
jodi (principal > 500000) tahole {
    interest_rate = 12
    dekhao "High amount - Interest rate: 12%"
} nahole {
    jodi (principal > 100000) tahole {
        interest_rate = 10
        dekhao "Medium amount - Interest rate: 10%"
    } nahole {
        interest_rate = 8
        dekhao "Small amount - Interest rate: 8%"
    }
}

dhori simple_interest = principal * interest_rate * years / 100
dhori total_amount = principal + simple_interest
dhori monthly_payment = total_amount / (years * 12)

dekhao "Simple Interest:"
dekhao simple_interest
dekhao "Total Amount:"
dekhao total_amount
dekhao "Monthly Payment:"
dekhao monthly_payment
```

### Example 8: Fuel Efficiency Calculator

```banglish
// Car fuel efficiency analysis
dhori distance_traveled = 500
dhori fuel_used = 25
dhori fuel_price_per_liter = 120

dhori mileage = distance_traveled / fuel_used
dhori total_fuel_cost = fuel_used * fuel_price_per_liter
dhori cost_per_km = total_fuel_cost / distance_traveled

dekhao "Trip Analysis:"
dekhao "Distance traveled (km):"
dekhao distance_traveled
dekhao "Fuel used (liters):"
dekhao fuel_used

dekhao "Fuel efficiency (km/l):"
dekhao mileage

dekhao "Total fuel cost:"
dekhao total_fuel_cost
dekhao "Cost per km:"
dekhao cost_per_km

// Efficiency rating
jodi (mileage > 20) tahole {
    dekhao "Excellent fuel efficiency!"
} nahole {
    jodi (mileage > 15) tahole {
        dekhao "Good fuel efficiency"
    } nahole {
        jodi (mileage > 10) tahole {
            dekhao "Average fuel efficiency"
        } nahole {
            dekhao "Poor fuel efficiency - consider a more efficient vehicle"
        }
    }
}
```

### Example 9: Number Guessing Game Logic

```banglish
// Number guessing game mechanics
dhori secret_number = 42
dhori player_guess = 35
dhori attempts = 3

dekhao "Number Guessing Game"
dekhao "Secret number (hidden):"
dekhao secret_number
dekhao "Your guess:"
dekhao player_guess
dekhao "Attempts remaining:"
dekhao attempts

jodi (player_guess == secret_number) tahole {
    dekhao "🎉 Congratulations! You guessed correctly!"
    dhori bonus_points = attempts * 10
    dekhao "Bonus points:"
    dekhao bonus_points
} nahole {
    jodi (player_guess < secret_number) tahole {
        dhori difference = secret_number - player_guess
        dekhao "📈 Too low! Try a higher number"
        dekhao "You were off by:"
        dekhao difference
        
        jodi (difference <= 5) tahole {
            dekhao "Very close!"
        } nahole {
            jodi (difference <= 15) tahole {
                dekhao "Getting warmer"
            } nahole {
                dekhao "Way off!"
            }
        }
    } nahole {
        dhori difference = player_guess - secret_number
        dekhao "📉 Too high! Try a lower number"
        dekhao "You were off by:"
        dekhao difference
        
        jodi (difference <= 5) tahole {
            dekhao "Very close!"
        } nahole {
            jodi (difference <= 15) tahole {
                dekhao "Getting warmer"
            } nahole {
                dekhao "Way off!"
            }
        }
    }
}

dhori remaining_attempts = attempts - 1
dekhao "Attempts left:"
dekhao remaining_attempts
```

### Example 10: BMI Calculator

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
    jodi (bmi < 25) tahole {
        dekhao "Category: Normal weight"
        dekhao "Recommendation: Maintain current weight"
    } nahole {
        jodi (bmi < 30) tahole {
            dekhao "Category: Overweight"
            dekhao "Recommendation: Consider losing some weight"
        } nahole {
            dekhao "Category: Obese"
            dekhao "Recommendation: Consult a healthcare provider"
        }
    }
}

// Calculate ideal weight range (for height)
dhori ideal_weight_min = 18.5 * height_m * height_m
dhori ideal_weight_max = 24.9 * height_m * height_m

dekhao "Ideal weight range:"
dekhao ideal_weight_min
dekhao "to"
dekhao ideal_weight_max
```

## 🔧 Advanced Features

### Nested If-Else Statements

Banglish supports unlimited nesting of conditional statements:

```banglish
jodi (condition1) tahole {
    jodi (condition2) tahole {
        jodi (condition3) tahole {
            dekhao "All conditions true"
        } nahole {
            dekhao "Only first two conditions true"
        }
    } nahole {
        dekhao "Only first condition true"
    }
} nahole {
    dekhao "First condition false"
}
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

**Happy Coding with Banglish! 🎉**

*Made with ❤️ for the Bengali programming community*
