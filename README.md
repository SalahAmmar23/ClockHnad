# ClockHnad


# ⏰ Digital Clock Simulation (Java)

This project simulates a **24-hour digital clock** using simple Java classes. The program continuously prints time from `00:00:00` up to `23:59:59` and then loops back to `00:00:00`.

---

## 📂 Files

### `Main.java`
The main class that runs the clock. It creates `ClockHand` objects for hours, minutes, and seconds, and updates them inside an infinite loop.

### `ClockHand.java`
A helper class that represents a single "hand" of a clock (like seconds, minutes, or hours). It knows how to:
- Advance its value by one
- Reset to zero when it reaches its limit
- Format its value as a two-digit string

---

## 🔧 How It Works

1. **Initialization**:
   - Hours: `ClockHand(24)`
   - Minutes: `ClockHand(60)`
   - Seconds: `ClockHand(60)`

2. **Infinite Loop**:
   - Prints the time in `HH:MM:SS` format
   - Advances the `seconds`
   - If `seconds` reach `60` (wraps to `0`), advances the `minutes`
   - If `minutes` reach `60` (wraps to `0`), advances the `hours`

---

## 🧪 Sample Output

```
00:00:00
00:00:01
00:00:02
...
23:59:59
00:00:00
```

This repeats forever like a real digital clock.

---

## 🎯 Concepts Learned

- Object-oriented programming
- Encapsulation (`ClockHand`)
- Infinite loops
- Time simulation logic
- Formatting output (`toString`)

---

Let me know if you want a version that runs for a few seconds only or with a real-time 1-second delay using `Thread.sleep(1000)`.