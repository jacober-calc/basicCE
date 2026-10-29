# TI-BASIC Wage Calculator

Simple calculator for computing hours worked and wages earned.

## What It Does

Calculates hours worked and pay based on start/end times in H.MM format (where .45 means 45 minutes, not 0.45 hours).

## Usage

1. Run the program
2. Enter start time in H.MM format (e.g., 8.30 for 8:30)
3. Enter end time in H.MM format (e.g., 17.15 for 5:15 PM)
4. Program displays:
   - Hours worked (in H.MM format)
   - Pay earned (in dollars)

## How It Works

The program uses a two-step process to avoid floating point errors:

1. **Convert inputs to decimal hours**
   - Extracts hours: `iPart(X)`
   - Converts minutes to decimal: `fPart(X)*100/60`
   - Example: 8.45 → 8 + (45/60) = 8.75 hours

2. **Calculate in decimal hours**
   - Subtracts start from end time
   - Multiplies by hourly wage ($18.25 default)
   - Rounds wage to cents

3. **Display conversion**
   - Converts decimal hours back to H.MM for display only
   - Example: 8.75 hours → 8.45 (8 hours 45 minutes)

## Configuration

Change the wage rate by editing the first line:
```
18.25→θ
```

Replace `18.25` with your hourly rate.