# ✅ What is Bash Scripting?
Think of Bash scripting like writing a to-do list for your computer. Instead of doing things one by one (like opening files or checking updates), you write instructions and say:
"Hey computer, follow these steps — and do them every time I run this script."

## 📄 The Basics: Your First Script
Imagine you're writing a note to yourself:
"When I wake up, I’ll brush my teeth and drink water."
In Bash, that’s:
```bash
#!/bin/bash
echo "Brushing teeth"
echo "Drinking water"
```
To run it, you save it as `morning.sh` and do:
```bash
chmod +x morning.sh   # permits it to run
./morning.sh          # runs the script
```

## 🧠 Variables (Like Storage Boxes)
A variable is like a label on a jar — it holds something.
Example: Saving someone’s name.
```bash
name="John"
echo "Good morning, $name"
```
💡 Real-life: Think of writing “Milk” on a jar. Then you can say “Hey, give me what’s in the ‘Milk’ jar.” That’s what Bash does with `$name`.

## ❓If Statements (Like Decision Making)
“If it's raining, carry an umbrella. Otherwise, wear sunglasses.”
```bash
weather="rainy"

if [ "$weather" = "rainy" ]; then
  echo "Carry an umbrella"
else
  echo "Wear sunglasses"
fi
```
💡 Real-life: Just like you check the weather before going out, Bash checks conditions before deciding what to do.

## 🔁 Loops (Doing Things Repeatedly)
“Do 10 push-ups every morning.”
```bash
for i in {1..10}; do
  echo "Push-up $i"
done
```
💡 Real-life: It's like setting an alarm to repeat every day — the computer does something over and over.

## 🧰 Functions (Reusable Actions)
“Every time I meet someone, I greet them with ‘Hello [name]!’”
```bash
greet() {
  echo "Hello, $1"
}

greet "Jane"
greet "Alex"
```
💡 Real-life: You create a greeting machine. You just pass a name, and it handles the rest.

## 🧳 Script Arguments (Like Giving Input)
“Pack a bag with these items: socks, charger, shirt”
You write:
```bash
echo "Packing $1"
echo "Packing $2"
echo "Packing $3"
```
Run it like:
```bash
./pack.sh socks charger shirt
```
💡 Real-life: You give your list once, the script handles it.

## 🧼 Cleaning Example: Real-World Use Case
Let’s say every day you clean your Downloads folder.
```bash
#!/bin/bash
echo "Cleaning Downloads folder..."
rm -rf ~/Downloads/*
echo "Done!"
```
💡 Now your script is your housekeeper.

## 🔚 Wrap-Up
Think of Bash as your personal assistant:
- 🧠 You give it a script = a clear list of steps
- ⚙️ It does all the boring stuff for you
- 💡 You can reuse it anytime

## 🧵 STRING COMPARISON OPERATORS
| Operator | Meaning             | Example                 |
|----------|---------------------|-------------------------|
| =        | Equal to            | `[ "$a" = "hello" ]`    |
| !=       | Not equal to        | `[ "$a" != "world" ]`   |
| <        | Less than (lexical) | `[ "$a" \< "$b" ]`     |
| >        | Greater than        | `[ "$a" \> "$b" ]`     |
| -z       | String is empty     | `[ -z "$a" ]`           |
| -n       | String is not empty | `[ -n "$a" ]`           |

⚠️ In `[ ... ]` you must escape `<` and `>` with `\`, but in `[[ ... ]]` you don’t need to:
```bash
[[ "$a" < "$b" ]]  # works without escaping
```

## 🔢 NUMERIC COMPARISON OPERATORS
| Operator | Meaning           | Example         |
|----------|-------------------|------------------|
| -eq      | Equal to          | `[ "$a" -eq 5 ]` |
| -ne      | Not equal to      | `[ "$a" -ne 10 ]`|
| -lt      | Less than         | `[ "$a" -lt 100 ]`|
| -le      | Less or equal     | `[ "$a" -le 3 ]` |
| -gt      | Greater than      | `[ "$a" -gt 7 ]` |
| -ge      | Greater or equal  | `[ "$a" -ge 18 ]`|

✅ BONUS: Use `(( ... ))` for numbers (cleaner)
```bash
a=5
b=10

if (( a < b )); then
  echo "a is less than b"
fi
```
✅ No need to quote variables or use `-lt`, `-eq`, etc.
