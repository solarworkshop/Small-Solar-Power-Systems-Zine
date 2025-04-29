# Small Solar Power Systems Workshop

## Basic Component Layout

![](file:///Users/p/Documents/solar%20zine/images/basic-setup.png)

## Voltage Drop Chart

This table provides the **maximum one-way wire run** (in feet) for a **3% voltage drop**, based on current load and wire gauge. Values are for **copper wire** and assume a **12V system**.

![](file:///Users/p/Documents/solar%20zine/images/volt-drop-12v.jpg)

## Key Electrical Concepts

When water flows through a pipe, increasing or decreasing either the size of the pipe or the flow rate of the water will accordingly increase or decrease the ammount of water you get out of the end of the pipe. Let’s look at three electrical concepts and how they relate to the water in the pipe:

**Voltage** (V_)_ - (measured in **volts**, represented as V) is the electrical potential, or size of the pipe. It’s not exactly correct, but it helps to think of it as a bigger pipe means there’s a bigger potential amount of water that could flow through, and a higher voltage the larger potential for electricity you have.

**Current** (I) - (measured in **amps**, represented as A) is the rate at which electrons flow through a circuit, or in the pipe how fast water is moving through it. The faster then water flows, the more water you have at the end. The higher the current (or amperage or amps) the more eletricity you have.

**Power** (P) - (measured in **watts**, represented as W) is the ammount of electricity used or produced. So in the pipe it’s the ammount or volume of water you get out at the end of the pipe.

**Resistance** (R) - (measured in **ohms**, represented as Ω) The opposition to the flow of electric current. So in our water example it’s any kink or obstruction in the pipe.

## Formulas

### Power

```mathjax
  Power(P) = Voltage(V) \times Current(I)
```

It might also be useful to think of it or remember it by the units of measure like:

```mathjax
  Watts (W) = Volts (V) \times Amps (A)
```

You can find voltage if you have current and power (_V = P/I_) or current if you have voltage and power (I = P/V).

### Amp-Hours (Ah)

An **Amp-Hour** (Ah) is a unit that measures **electrical charge capacity** over time. It tells you how much current a battery can supply for **one hour** before it is depleted.

```mathjax
  AmpHours(Ah) = Current (A) \times Time (hours)
```

### Watt-Hours (Wh)s

A **Watt-Hour (Wh)** is a measure of **energy**. It tells you **how much power a system can deliver over time**. Since power is measured in watts (W), Watt-Hours indicate the total energy available.

## Multimeter Layout

![](file:///Users/p/Documents/solar%20zine/images/multimeter.png)

## Measuring Voltage with a Multimeter

#### Step 1: Set the Multimeter to DC Voltage Mode

- Turn the dial to the **DC voltage (V⎓)** setting.
- Select a voltage range **higher than expected**:
- For a **12V battery**, set it to **20V DC** (if available).
- For a **24V, 36v, or 48v system**, set it to **200V DC**.

#### Step 2: Insert the Test Leads

- Black probe → COM (Common) port
- Red probe → V (Voltage) port

#### Step 3: Check Polarity and Voltage

- **Red probe** to the **positive (+) terminal**.
- **Black probe** to the **negative (-) terminal**.
- Read the display:
- **Positive reading (e.g., 12.6V)** → Polarity is correct.
- **Negative reading (e.g., -12.6V)** → Probes are reversed. Swap them to identify the correct polarity.

## Parallel vs. Series

Parallel Wiring: Same Voltage, More Current
Series Wiring: More Voltage, Same Current

![](file:///Users/p/Documents/solar%20zine/images/parallel-series.png)

## Solar Panel Measurements

| **Label Term** | **What It Means** | **Typical Values (Example for a 100W Panel)** |
| --- | --- | --- |
| **Max Power (Pmax)** | The maximum wattage output under ideal conditions. | **100W** |
| **Voltage at Max Power (Vmp)** | The voltage the panel produces under load (when connected to a system). | **18V - 20V** |
| **Current at Max Power (Imp)** | The current (amps) the panel produces under load. | **5A - 6A** |
| **Open Circuit Voltage (Voc)** | The voltage when the panel is not connected to anything (no load). | **22V - 24V** |
| **Short Circuit Current (Isc)** | The maximum current the panel can produce when shorted. | **5.5A - 6.5A** |
| **Operating Voltage Range** | The panel’s recommended working range. | **12V (nominal) or 24V (nominal)** |

## Battery Measurements


| Measurement           | Definition                                                   | Expressed As            | Why It Matters                                                           | Example                                                   |
|-----------------------|--------------------------------------------------------------|-------------------------|--------------------------------------------------------------------------|-----------------------------------------------------------|
| **Depth of Discharge (DoD)** | How much energy you can safely use before recharging.       | Percentage (%)          | Batteries last longer if not fully discharged. Lead-acid: ~50%; Lithium: ~80–90%. | Lead-acid: 50% DoD; Lithium: 80-90% DoD                   |
| **State of Charge (SoC)**    | How full the battery currently is.                         | Percentage (%)          | Helps prevent over-discharge and ensures battery health.                 | Fully charged = 100%; fully empty = 0%                    |
| **C-Rate** (Charge/Discharge Rate) | The speed at which a battery is charged or discharged relative to its capacity. | Number (1C, 0.5C, etc.) | Charging/discharging too fast can shorten battery life or cause damage.  | 1C: full charge/discharge in 1 hour; 0.5C: in 2 hours     |
| **Cycle Life**               | Number of full charge/discharge cycles before battery capacity significantly decreases. | Number of cycles        | Indicates lifespan. Lithium generally has higher cycle life than lead-acid. | 500 cycles (typical lead-acid); 2000+ cycles (typical lithium) |