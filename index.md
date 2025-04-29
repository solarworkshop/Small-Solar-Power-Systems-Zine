---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

<!-- TOC start (generated with https://github.com/derlin/bitdowntoc) -->

- [Intro to Small Solar Power Systems](#intro-to-small-solar-power-systems)
- [Electricity](#electricity)
- [Overview of Solar Components](#overview-of-solar-components)
- [Planning Your System Capacity](#planning-your-system-capacity)
- [Planning Your System Wiring](#planning-your-system-wiring)
- [Putting Everything Together](#putting-everything-together)
- [Installation Longevity Considerations](#installation-longevity-considerations)
- [Alternative Ways to Charge Batteries](#alternative-ways-to-charge-batteries)
- [PV Panels In Depth](#pv-panels-in-depth)
- [Charge Controllers In Depth](#charge-controllers-in-depth)
- [Batteries In Depth](#batteries-in-depth)
- [Inverters In Depth](#inverters-in-depth)
- [Design and Wire a 12V Fuse Box](#design-and-wire-a-12v-fuse-box)
- [**Considerations for Bigger (than 12V) Systems**](#considerations-for-bigger-than-12v-systems)
- [**Tools, Connectors, and Other Hardware**](#tools-connectors-and-other-hardware)
- [12V Solar Systems Budget Examples](#12v-solar-systems-budget-examples)
- [Beginner Solar System Planning Checklist](#beginner-solar-system-planning-checklist)

<!-- TOC end -->

<!-- TOC --><a name="intro-to-small-solar-power-systems"></a>
# Intro to Small Solar Power Systems

![](https://raw.githubusercontent.com/solarworkshop/Small-Solar-Power-Systems-Zine/main/images/basic-setup.png)
version 0.1.1

This is a work in progress. Please email [solarworkshop@proton.me](mailto:solarworkshop@proton.me) with any feedback or if you want to help.

For digital version and more resources visit [linktr.ee/solarworkshop](https://linktr.ee/solarworkshop)

## Introduction

This zine for anyone at any skill level looking to build small solar power systems for power in remote locations, during disaster relief situations, or built into a vehicle. It is intended to cover as much as possible, but is far from exhaustive about any of these topics. It also assumes you’re starting out having never done anything with electricity at all. Which is fine, because we believe these are skills anyone can learn.

By small we mean systems for powering lights, laptops, phones, radios, and the like, not for powering your a whole house or household appliances. If you do want to build bigger systems, this is still a fine place to start.

## Saftey

I’ve often heard “I just don’t mess with electrical stuff because it scares me” so I want to touch on electrical saftey briefly first in hope that you feel empowered to play with eletricity and learn in a safe way. There is a lot more to this topic, but we’re going to touch on some basics as they pertain to small solar setups.

First, it is good to have a healthy fear of electricity. It can be deadly and its really good at starting fires. However, when working with the relativley low DC current and voltage that we are it is very unlikely that you’ll be shocked ever.

Here are some basics that will ensure you are safe. If you’ve never worked with electricity before some of the concepts here may not make sense, but don’t worry they’ll be explained later on and then you can come back to this section.

- Keep longer exposed metal tools away from battery terminals, touching them to both will cause an arc and huge spark that can result in fragments of metal flying into your eyes.
- For that reason it is typically recommended that you wear eye protection when doing this work, but most people don’t and you just have to be careful.
- Do not cross positive and negative wires. It’s a good idea to use different color wires (typically red for positive and black for negative) to avoid confusion.
- Touching one battery terminal or live wire should not hurt you in anything we are doing here, but it’s still best to avoid it.
- Avoid touching two battery terminals or places in the system at the same time.
- Ensure that all connections are electrical connections you make are tight and snug so they don’t move or come loose.
- Avoid having exposed loose wires in or near your system when it is powered. Keeping your work neat is important for saftey.
- Avoid running wires through areas where they will be exposed to friction, sharp edges, or other environmental factors that could damange their insulation.
- If you are unsure if there is power going through something or what it’s polarity is (what wire is positive / negative) check it’s polarity with a multimeter first.
- Work slowly, carefully, and deliberatley. Think about what wire you are connecting where and why, so you don’t make mistakes.
- Use properly sized wire thicknesses. Too small of wires will heat up and catch fire.
- Use properly sized fuses and breakers to protect from short circuit and wires heating up.
- Although we’re mostly working with DC power here, we still get into AC - what houses have - and the same rules apply for AC as they do in a house. If you touch the hot wire or stick something in a socket you will get zapped.
- This should go without saying, but do not work with eletricity in wet conditions.

<!-- TOC --><a name="electricity"></a>
# Electricity

Electricity is the flow of electric charge through a conductor, such as a wire.

Electricity occurs due to the movement of electrons, which are negatively charged particles found in atoms. When electrons move from one atom to another in a controlled way, an electric current is created.

## What Is a Circuit?

A circuit is simply a pathway that allows electricity to flow from a power source (like a battery or solar panel), through wires and devices (such as lights, appliances, or other loads), and back to the power source.

For electricity to move and do useful work, the circuit must be complete — meaning there is a continuous path with no breaks. If the circuit is broken (like when a switch is turned off or a wire is disconnected), the flow of electricity stops.

At its core, a circuit includes three basic parts:

- Power Source: Provides the energy (e.g., a battery, solar panel, or generator).

- Conductors: Wires that carry the electrical current.

- Load: Any device that uses the electricity (like a light bulb, fan, or pump).

### How a Basic Circuit Works

- Power flows from the positive terminal of the source.

- Current moves through the wire to the load (doing work, like lighting a bulb).

- Current returns to the negative terminal of the source, completing the loop.

Think of it like water flowing through a hose: the pump (power source) pushes water (electricity) through the hose (wire), spins a water wheel (load), and then the water returns to the pump.

## Characteristic of Electricity

Let’s try to explain some key electrical concepts using the analogy of water flowing through a pipe.

When water flows through a pipe, increasing or decreasing either the size of the pipe or the flow rate of the water will accordingly increase or decrease the ammount of water you get out of the end of the pipe. Let’s look at three electrical concepts and how they relate to the water in the pipe:

**Voltage** (V_)_ - (measured in **volts**, represented as V) is the electrical potential, or size of the pipe. It’s not exactly correct, but it helps to think of it as a bigger pipe means there’s a bigger potential amount of water that could flow through, and a higher voltage the larger potential for electricity you have.

Voltage can also be helpful to think about in terms of compatability of different components in a circuit. A circuit with components rated for different voltages will not work and may cause damage or fires. Components even of the same voltage that are meant for AC or DC power (which will be covered later) also cannot be mixed. For example, pretty much everything in a vehicle is 12 volts DC, while most everything in your house is 120 volts AC. 

**Current** (I) - (measured in **amps**, represented as A) is the rate at which electrons flow through a circuit, or in the pipe how fast water is moving through it. The faster then water flows, the more water you have at the end. The higher the current (or amperage or amps) the more eletricity you have.

**Power** (P) - (measured in **watts**, represented as W) is the ammount of electricity used or produced. So in the pipe it’s the ammount or volume of water you get out at the end of the pipe.

_Bonus that you probably won’t use for our purposes but you might as well know:_

**Resistance** (R) - (measured in **ohms**, represented as Ω) The opposition to the flow of electric current. So in our water example it’s any kink or obstruction in the pipe.

## Power Formula

There is one important relationship amung these concepts that will help you immensly in working on solar power projects (and probably your every day life if you ever look at electrical appliance labels). But that means we have to introduce a formula - the formula for power. Remember power is just the amount of water you get at the end of the pipe once you’ve adjusted the size of the pipe and the flow rate of the water.

### $`Power(P) = Voltage(V) \times Current(I)`$


It might also be useful to think of it or remember it by the units of measure like:

### $`Watts (W) = Volts (V) \times Amps (A)`$

All you do to get power (watts) is multiple voltage (volts) by current (amps). Wattage tells you how much electricity something will use without knowing the volts or amps.

The power formula also allows you to find voltage if you have current and power (_V = P/I_) or current if you have voltage and power (I = P/V).

### Power Formula in Practice

Let’s see why this formula is useful. Suppose you have a USB charger that says it’s rated to 30 watts. We also know that USB devices are all 5 volts.

## Adding the Hours Measure

When designing a **small solar power system**, it’s essential to understand **Amp-Hours** (Ah) and **Watt-Hours** (Wh) to measure battery capacity and energy consumption.

### Amp-Hours (Ah)

An **Amp-Hour** (Ah) is a unit that measures **electrical charge capacity** over time. It tells you how much current a battery can supply for **one hour** before it is depleted.

### $`AmpHours(Ah) = Current (A) \times Time (hours)`$

**Example:**

- A **100Ah battery** can provide:
- **100A for 1 hour**, or
- **10A for 10 hours**, or
- **1A for 100 hours**

However, this depends on **battery efficiency and discharge rate**.

### Watt-Hours (Wh)s

A **Watt-Hour (Wh)** is a measure of **energy**. It tells you **how much power a system can deliver over time**. Since power is measured in watts (W), Watt-Hours indicate the total energy available.

#### **Formula:**

### $`WattHours (Wh) = Volts (V) \times AmpHours (Ah)`$

#### **Example:**

- A **12V 100Ah battery** has: 

### $`12V \times 100Ah = 1,200Wh`$

This means the battery can **deliver 1,200 watts for 1 hour** or **100 watts for 12 hours** (under ideal conditions).

#### Key Differences Between Ah and Wh

| **Unit** | **Measures** | **Formula** | **Usage** |
| --- | --- | --- | --- |
| **Amp-Hours (Ah)** | Electrical charge capacity | `Ah = A × hours` | Battery size (capacity) |
| **Watt-Hours (Wh)** | Total energy stored or consumed | `Wh = V × Ah` | Energy usage of devices |

#### Why Are These Important in Solar Power Systems?

- **Choosing the Right Battery Size:** Batteries are rated in **Ah**, but energy needs are often in **Wh**.
- **Estimating Energy Consumption:** Devices use **Wh** (e.g., a 50W fan for 5 hours = 250Wh).
- **System Efficiency:** Inverters and other components affect how much of the stored **Wh** can actually be used.

## AC vs. DC Power

Electricity can flow in two different ways: **Alternating Current (AC)** and **Direct Current (DC)**. Both are used in electrical systems but have different characteristics and applications. You do not need to really know any of this for the rest of our purposes; besides that we will be using mostly DC unless otherwise specificed, and that AC and DC power are not interchangable or mixable.

![](https://raw.githubusercontent.com/solarworkshop/Small-Solar-Power-Systems-Zine/main/images/dc_vs_ac.png)

### Alternating Current (AC)

AC power **changes direction periodically**, meaning the voltage alternates between positive and negative. In most household and industrial systems, AC switches direction **50 or 60 times per second (50 Hz or 60 Hz)**.

#### Characteristics of AC:

- Reverses direction in a sine wave pattern.
- Easier to transmit over long distances with minimal energy loss.
- Standard for grid electricity used in homes, businesses, and industries.

### Direct Current

DC power **flows in only one direction**, with a constant voltage level. It is commonly used in **batteries, solar panels, and low-voltage electronics**.

#### **Key Characteristics of DC:**

- Maintains a constant voltage level (does not alternate).
- Efficient for storage in batteries.
- Common in small-scale and off-grid power systems.
- Common uses include: solar power systems, batteries in cars, laptops, and phones, LED lighting, and small electronics.

## Polarity

**Polarity** refers to the positive (**+**) and negative (**\-**) orientation of a DC circuit. Unlike AC power, which alternates direction, **DC electricity flows in only one direction**.

- **Correct polarity** ensures that devices receive power properly.
- **Reversed polarity** can damage sensitive electronics, prevent charging, or cause a short circuit.
- In solar power systems, **battery terminals, solar panels, and charge controllers must be connected with correct polarity** for efficient operation and safety.

A multimeter can help confirm **polarity** before making connections.

### Why Checking Polarity Matters

**Prevents damage to electronics** – Some DC devices can be permanently damaged if connected backward.  
**Ensures proper battery and solar panel connections** – Incorrect polarity can prevent charging or damage charge controllers.  
**Avoids wiring mistakes in DIY solar systems** – Double-checking polarity before connecting wires prevents costly errors.

## Multimeters

A **multimeter** is an essential tool for measuring **DC voltage** in a small solar power system. It helps check the voltage of batteries, solar panels, and other DC components to ensure they are functioning correctly.

![](https://raw.githubusercontent.com/solarworkshop/Small-Solar-Power-Systems-Zine/main/images/multimeter.png)

### Measuring DC Voltage & Checking Polarity

#### Step 1: Set the Multimeter to DC Voltage Mode

- Turn the dial to the **DC voltage (V⎓)** setting.
- Select a voltage range **higher than expected**:
- For a **12V battery**, set it to **20V DC** (if available).
- For a **24V, 36v, or 48v system**, set it to **200V DC**.
- If your multimeter has **auto-ranging**, it will adjust automatically.

#### Step 2: Insert the Test Leads

- Black probe → COM (Common) port
- Red probe → V (Voltage) port

#### Step 3: Check Polarity and Voltage

- **Red probe** to the **positive (+) terminal**.
- **Black probe** to the **negative (-) terminal**.
- Read the display:
- **Positive reading (e.g., 12.6V)** → Polarity is correct.
- **Negative reading (e.g., -12.6V)** → Probes are reversed. Swap them to identify the correct polarity.


<!-- TOC --><a name="overview-of-solar-components"></a>
# Overview of Solar Components

A small solar power system consists of several key components that work together to **capture, store, and distribute electricity**. Understanding these components is essential for designing an efficient and reliable system.


### 1\. Solar Panels (Photovoltaic Modules)

**Function:** Convert sunlight into DC electricity.

- Made of **solar cells** (typically silicon-based).
- Rated by **wattage (W)**, indicating power output in ideal sunlight.
- Types: **Monocrystalline, Polycrystalline, Thin-Film** (varying efficiency & cost).

### 2\. Charge Controller

![](https://raw.githubusercontent.com/solarworkshop/Small-Solar-Power-Systems-Zine/main/images/charge-controllers.jpg)

**Function:** Regulates the power from solar panels to **prevent overcharging** the battery. Can also help prevent battery from being over discharged.

- **PWM (Pulse Width Modulation):** Basic and budget-friendly. 
- **MPPT (Maximum Power Point Tracking):** More efficient, extracts more power.

### 3\. Battery

![](https://raw.githubusercontent.com/solarworkshop/Small-Solar-Power-Systems-Zine/main/images/batteries.png)

**Function:** Stores energy for use when the sun isn’t shining. The two most popular options are:

- **Lead-Acid (AGM, Gel):** Affordable but lower lifespan.
- **Lithium-Ion (LiFePO₄):** More efficient, longer-lasting, but higher cost.

### 4\. Inverter

![](https://raw.githubusercontent.com/solarworkshop/Small-Solar-Power-Systems-Zine/main/images/inverters.png)

**Function:** Converts **DC power (from batteries/solar panels) into AC power** for household appliances.

- **Pure Sine Wave:** Best for sensitive electronics.
- **Modified Sine Wave:** Cheaper but may not work with all devices.
- Rated in **watts (W)** to match appliance power needs.


(See **Pure vs. Modified Sine Wave Inverters** in the **Sourcing Components** section later for more details about how each of these work.)
### 5\. Wiring and Fuses

**Function:** Safely connects and protects system components.

- **Proper gauge wires** prevent voltage drop & overheating.
- **Fuses and circuit breakers** protect against overcurrent.

- **Connectors (MC4, Anderson, etc.)** ensure secure wiring.

### 6\. Optional Components

- **Battery Monitor:** Tracks battery voltage and charge level.
- **Solar Disconnects:** Safety switches for maintenance.

<!-- TOC --><a name="planning-your-system-capacity"></a>
# Planning Your System Capacity

This is an example of how you would plan and figure out the components needed for a system that can run two ham radios and a light.

### Step 1: Determine Total Power Needs

1. List all radios and accessories.
2. Find each device’s **power rating (W)** and **operating hours per day**.
3. Use the formula:

### $`Total Energy (Wh) = ∑(Power(W) × Hours Per Day)`$

This is the sum of the watt hours of each device.

**Example Setup:**

| **Device** | **Power (W)** | **Hours per Day** | **Energy (Wh)** |
| --- | --- | --- | --- |
| HF Transceiver | 50W | 3h  | 150Wh |
| VHF/UHF Radio | 25W | 4h  | 100Wh |
| LED Light | 10W | 5h  | 50Wh |
| **Total Energy Needed** |     |     | **300Wh/day** |

### Step 2: Choose a Solar Panel

- Find your **average sunlight hours** (there are websites where you can look this up, in the mid-atlantic its 3.5 - 4 peak sunlight hours per day).
- Use the formula:

Solar Panel Size (W) = Daily Energy (Wh) / Sunlight Hours

**Example:  
**For **300Wh/day** and **5 sunlight hours**: 300Wh / 5h = 60W

**Use a 100W solar panel** for extra capacity and cloudy days.

### Step 3: Select a Battery

- Convert **Wh to Ah** for a **12V battery**:

Battery Capacity(Ah) = Daily Energy (Wh) / Battery Voltage (V)

**Example:** 300Wh / 12V = 25Ah

**Use a 50Ah deep-cycle battery** to ensure reliable backup power.

### Step 4: Pick a Charge Controller

- Prevents overcharging and regulates power.
- Use the formula:

Charge Controller (A) = Solar Panel (W) / Battery Voltage (V)

**Example:**

100W / 12V = 8.3A

**Use a 10A or 15A charge controller** for safety.

### Step 5: Consider Extra Power for Accessories

- If running **a laptop, fan, or additional radios**, increase **battery size** to **75Ah–100Ah**.
- If using **higher power modes (SSB, FM, digital)**, allow extra power margin.

### Recommended Components for Ham Radios

| **Component** | **Size** |
| --- | --- |
| **Solar Panel** | 100W–200W |
| **Battery** | 12V 40Ah–100Ah |
| **Charge Controller** | 10A–15A |

<!-- TOC --><a name="planning-your-system-wiring"></a>
# Planning Your System Wiring

Before we put everything together there are some more details we need to work out. We need to determine what were wiring in parallel or series, the type and size of the wire, and what fuses or breakers well need.

### Parallel vs. Series

Wiring **solar panels** and **batteries** in series or parallel affects the **voltage and current** of the system. Understanding the differences helps in designing an efficient **12V solar power system**.

![](https://raw.githubusercontent.com/solarworkshop/Small-Solar-Power-Systems-Zine/main/images/parallel-series.png)

#### Parallel vs. Series Wiring for Solar Panels

##### Parallel Wiring (Same Voltage, More Current)

- **How It Works:** Connect all **positive terminals** together and all **negative terminals** together.
- **Effect:** **Voltage stays the same**, but **current (amperage) adds up**.

**Best For:** 12V systems where multiple panels charge a 12V battery.

**Example:** Connecting **two 100W (12V, 8.3A) panels** in parallel:

| **Panel** | **Voltage (V)** | **Current (A)** | **Total Power (W)** |
| --- | --- | --- | --- |
| Panel 1 | 12V | 8.3A | 100W |
| Panel 2 | 12V | 8.3A | 100W |
| **Total (Parallel)** | **12V** | **16.6A** | **200W** |

###### How to Use Solar Y-Splitters in Parallel Installation

Solar Y-splitters are **two-to-one connectors** that allow you to **combine multiple solar panels in parallel** easily. They typically come in **MC4-compatible** versions with:

- **One male and two female connectors** (for positive connections).
- **One female and two male connectors** (for negative connections).

##### Series Wiring (More Voltage, Same Current)

- **How It Works:** Connect the **positive terminal of one panel** to the **negative terminal of the next**.
- **Effect:** **Voltage adds up**, but **current stays the same**.

**Best For:** Higher-voltage systems (24V, 48V) for long cable runs with less energy loss.

**Example:** Connecting **two 100W (12V, 8.3A) panels** in series:

| **Panel** | **Voltage (V)** | **Current (A)** | **Total Power (W)** |
| --- | --- | --- | --- |
| Panel 1 | 12V | 8.3A | 100W |
| Panel 2 | 12V | 8.3A | 100W |
| **Total (Series)** | **24V** | **8.3A** | **200W** |

#### Parallel vs. Series Wiring for Batteries

##### Parallel Battery Wiring (Same Voltage, More Capacity)

- **How It Works:** Connect all **positive terminals** together and all **negative terminals** together.
- **Effect:** **Voltage remains the same**, but **amp-hours (Ah) increase**.

**Best For:** Expanding battery capacity while keeping the system at **12V**.

**Example:** Connecting **two 12V 50Ah batteries** in parallel:

| **Battery** | **Voltage (V)** | **Capacity (Ah)** | **Total Energy (Wh)** |
| --- | --- | --- | --- |
| Battery 1 | 12V | 50Ah | 600Wh |
| Battery 2 | 12V | 50Ah | 600Wh |
| **Total (Parallel)** | **12V** | **100Ah** | **1,200Wh** |

#### Series Battery Wiring (More Voltage, Same Capacity)

- **How It Works:** Connect the **positive terminal of one battery** to the **negative terminal of the next**.
- **Effect:** **Voltage adds up**, but **Ah remains the same**.

**Best For:** 24V or 48V systems to support larger inverters with **lower current draw**.

**Example:** Connecting **two 12V 50Ah batteries** in series:

| **Battery** | **Voltage (V)** | **Capacity (Ah)** | **Total Energy (Wh)** |
| --- | --- | --- | --- |
| Battery 1 | 12V | 50Ah | 600Wh |
| Battery 2 | 12V | 50Ah | 600Wh |
| **Total (Series)** | **24V** | **50Ah** | **1,200Wh** |

#### Choosing Parallel vs. Series

| **Factor** | **Parallel** | **Series** |
| --- | --- | --- |
| **Voltage Output** | Same as one unit | Adds up |
| **Current (Amps)** | Adds up | Same as one unit |
| **Best For** | 12V systems, increasing battery capacity | 24V+ systems, reducing current loss |
| **Cable Thickness** | Thicker cables needed for high amps | Thinner cables possible due to lower amps |
| **Charge Controller Type** | PWM (low cost) or MPPT | MPPT (required for series solar panels) |

#### Hybrid (Series-Parallel) Wiring

For **larger systems**, both **series and parallel** wiring can be combined.

**Example:**

- **Four 100W solar panels (12V, 8.3A each)**
- Two **series pairs** → Each pair becomes **24V, 8.3A**
- Then connect those two pairs in **parallel** → Final output **24V, 16.6A**

This balances **higher voltage for efficiency** while maintaining **high current output**.

### Types of DC Wire and Their Uses

This list is not exhaustive, but here are the common types of wire used in solar applications. You will likely need a combination of types and sizes of wires to build your system correctly

#### 1\. THHN (Thermoplastic High Heat Nylon-Coated) Wire

- **Use:** Common in industrial and home wiring, also be used in solar power systems.
- **Advantages:**
- Heat-resistant and durable.
- Has an outer nylon coating for extra protection.

#### 3\. Welding Cable

- **Use:** Heavy-duty **high-current applications**, such as battery banks and inverters.
- **Advantages:**
- Extremely flexible and resistant to wear.
- Can handle very high currents with minimal voltage drop.
- **Best For:** Connecting batteries, inverters, and large solar setups.

#### 5\. PV (Photovoltaic) Wire

- **Use:** Designed **specifically for solar panel connections**.
- **Advantages:**
- UV-resistant and weatherproof.
- Rated for high-voltage DC power transmission.
- **Best For:** Connecting solar panels to charge controllers.

#### 6\. Automotive Wire (GPT, GXL, TXL)

- **Use:** Found in **12V DC automotive and mobile power systems**.
- **Advantages:**
- Flexible and heat-resistant.
- Insulated for protection in engine compartments.
- **Best For:** Mobile solar power systems, vehicles, trailers.

#### Wire Types at a Glance

| **Wire Type** | **Best Used For** | **Advantages** |
| --- | --- | --- |
| THHN Wire | Outdoor runs, conduit installations | Heat-resistant, durable |
| Welding Cable | Battery banks, inverters | High-current capacity, flexible |
| PV Wire | Solar panel connections | UV/weather-resistant, safe for high voltage |
| Automotive Wire | 12V DC systems, mobile setups | Flexible, heat-resistant |

### Wire Size and Voltage Drop

Proper wire sizing is **critical** in a solar power system to **prevent overheating, reduce power loss, and maintain efficiency**. One of the biggest factors in choosing wire size is **voltage drop**, which occurs when electricity travels through the wire and loses energy due to resistance.

Voltage drop happens depending on the length of the wire, its thickness, and the voltage and current running through it. Wires that are too thin or run too long introduce more and more resistence, which causes the voltage to drop. This can impact performance or you system, but also can start fires as the electricity lost is displaced as heat.

Wire sizes are measured in AWG (American Wire Guage). The lower the guage number the thicker the wire and the higher the guage number the thinner.

In order to properly size your wires you will need to know the maximum possible current (amps) running through them.

- For solar panels just add up the amprage of each panel (or use the power formula to convert watts to amps).
- TODO: battery to battery, charge controller, inverter, loads (should this be it’s own section?)

This chart shows **wire gauges (AWG 00 to 18)** along with their **ampacity (current capacity)** and **common uses** in **DC solar power systems**.

| **AWG (Gauge)** | **Diameter (inches)** | **Ampacity (DC, Copper Wire)** | **Common Uses in Solar DC Systems** |
| --- | --- | --- | --- |
| **00 (2/0 AWG)** | 0.365 | 200A+ | **Battery to large inverter (2000W+), battery bank interconnects** |
| **0 (1/0 AWG)** | 0.325 | 175A | **Battery to mid-size inverter (1000W–2000W)** |
| **1 AWG** | 0.289 | 150A | **High-power charge controller to battery** |
| **2 AWG** | 0.258 | 125A | **Large battery-to-inverter cables (12V, 24V systems)** |
| **4 AWG** | 0.204 | 100A | **Battery to inverter (500W–1500W)** |
| **6 AWG** | 0.162 | 75A | **Charge controller to battery (up to 60A), medium inverter connections** |
| **8 AWG** | 0.128 | 50A | **Solar panel to charge controller (longer runs)** |
| **10 AWG** | 0.102 | 30-40A | **Solar panel strings, short charge controller runs** |
| **12 AWG** | 0.081 | 20-25A | **Smaller solar panel connections, LED lighting circuits** |
| **14 AWG** | 0.064 | 15-20A | **Low-power DC appliances, short solar runs (under 10A)** |
| **16 AWG** | 0.051 | 10-15A | **Small loads (USB ports, 12V accessories)** |
| **18 AWG** | 0.040 | 5-10A | **Low-current sensors, monitoring equipment** |

#### Determining Appropriate Wire Size

To detemine what size wire to use it’s best to use an online or phone based voltage drop calculator where you plug in the voltage, current (amps), and size of the wire run, and it gives you back the thickness you need to keep the voltage drop within the 3% maximum recommended drop range. You can also consult this table:

#### Maximum One-Way Wire Distance (Feet) for 3% Voltage Drop

This table provides the **maximum one-way wire run** (in feet) for a **3% voltage drop**, based on current load and wire gauge. Values are for **copper wire** and assume a **12V system**.

![](https://raw.githubusercontent.com/solarworkshop/Small-Solar-Power-Systems-Zine/main/images/volt-drop-12v.jpg)

#### Examples of Wire Sizing in a 12V System

**Example 1: Solar Panel to Charge Controller**

- **System:** 12V, 10A, 20 feet
- **Voltage drop target:** 3% of 12V = 0.36V
- **Wire needed:** **10 AWG**

**Example 2: Battery to Inverter (High Power)**

- **System:** 12V, 100A, 5 feet
- **Voltage drop target:** 3% of 12V = 0.36V
- **Wire needed:** **2/0 AWG** (very thick)

### Fuses and Breakers

#### What Are Fuses and Breakers?

Fuses and circuit breakers are essential safety components in a **12V solar power system**. They protect the wiring and components from damage due to overcurrent conditions (such as short circuits or overloads).

- **Fuses**: Single-use devices that "blow" or melt when the current exceeds a certain limit. Once blown, they must be replaced.
- **Breakers**: Reusable switches that "trip" when overcurrent is detected. They can be reset manually.

#### Where to Place Fuses and Breakers in a 12V Solar System

Fuses and breakers should be installed **as close as possible to the power source** (battery or charge controller) to protect wiring and devices downstream. Common locations include:

1. **Between the Solar Panels and Charge Controller**

- If your panels exceed the **amp rating** of your charge controller, install a fuse or breaker on the **positive wire** from the panels.
- Use a **breaker** here if you want an easy way to disconnect panels for maintenance.

**2\. Between the Charge Controller and Battery**

- Protects the **battery from overcurrent**.
- Size the fuse/breaker **slightly higher than the charge controller’s max output** (e.g., for a 30A controller, use a **35A fuse**).

**3\. Between the Battery and Inverter**

- The **largest fuse/breaker in the system** due to the high current draw of inverters.
- Install a fuse rated for **1.25× the inverter’s max current draw**. e.g., for a 1000W inverter at 12V:

### $`{1000W \over 12V} = 83A`$

### $`{83A \times 1.25} = 104A`$

So use /a **100A-125A fuse**.

**4\. Between the Battery and Fuse Block (for 12V Accessories)**

- A **main fuse** protects the wiring for **lights, USB ports, fridges, and other 12V loads**.
- Use a **breaker if you want an easy shutoff switch** for all accessories.

**5\. At Each 12V Accessory Circuit**

- Each **individual device should have its own fuse**.
- **Example fuse sizes**:
- **LED lights (5A circuit):** Use a **5A or 7.5A fuse**.
- **Fridge (10A circuit):** Use a **15A fuse**.
- **USB ports (3A circuit):** Use a **5A fuse**.

#### How to Determine Proper Fuse Size

1. Identify the wire gauge and ampacity (maximum current capacity).
2. Find the maximum current draw of the device.
3. Multiply by 1.25 (125%) to allow for startup surges.
4. Choose a fuse that does not exceed the wire’s ampacity.

**Example:** A 12V fridge draws **8A continuously**.

- **8A × 1.25 = 10A fuse**
- If using **14 AWG wire** (which handles **15A max**), a **10A fuse** is safe.

<!-- TOC --><a name="putting-everything-together"></a>
# Putting Everything Together

Now you know the components you’re using, the size or the wires and fuses or breakers needed, and how the batteries and panels will be laid out. So let’s put it all together, by reviewing the function of each component, how they are connected, and where they are place.

#### 1\. Solar Panels

- **Function**: Capture sunlight and generate DC electricity.
- **Connection**: Wired in **parallel** for 12V systems (voltage stays the same, current increases).
- **Placement**: Install on a roof, ground mount, or pole mount **facing the sun** for maximum exposure.

#### 2\. Solar Charge Controller

- **Function**: Regulates voltage and current from panels to prevent battery overcharging.
- **Connection**:
- **Solar Panels → Charge Controller (PV Input)**
- **Battery → Charge Controller (Battery Terminals)**
- **Fuse Between Battery and Controller (Close to Battery)**
- **Placement**: **Close to the battery** (within **3-5 feet**) to minimize voltage drop.

#### 3\. Battery Bank

- **Function**: Stores solar energy for use when sunlight is unavailable.
- **Connection**:
- **Charge Controller → Battery (Positive & Negative Terminals)**
- **Battery Fuse (Near Battery Positive Terminal)**
- **Placement**: In a **well-ventilated area** (especially for lead-acid batteries).

#### 4\. Inverter (Optional – For AC Loads)

- **Function**: Converts 12V DC to 120V AC for household appliances.
- **Connection**:
- **Battery → Inverter (With Inline Fuse or Breaker Near Battery)**
- **Inverter AC Output → Appliances**
- **Placement**: **Close to the battery** (within **3-5 feet**) to handle high current draw efficiently.

#### 5\. 12V Distribution (Fuse Block for DC Loads)

- **Function**: Distributes 12V DC power to lights, USB ports, and other accessories.
- **Connection**:
- **Battery → Fuse Block (With Main Fuse Between Them)**
- **Fuse Block → Individual Circuits (Lights, Fridge, etc.)**
- **Placement**: **Near the battery** but accessible for easy fuse replacement.

**Preparing the Wires and Making the Connections**

Now that we’ve reviewed the basics of how the system fits together again, let’s go over step by step how to connect each component, including how to prepare the wires and various connectors.

**Important:** When you strip wires and insert them in a screw terminal or crimp a ring terminal on a wire, make sure you strip just enough to fit so that no bare wire is exposed. Exposed bare wire increasing the chances of the wire becoming damaged or shorting / sparking.

#### 1\. Connecting Solar Panels

**Wiring Type:** Solar panels typically use **MC4 connectors** on their output wires. If the panel has bare wires, they may connect to the charge controller using **ring terminals, spade terminals, or screw terminals**.

#### How to Prepare the Wires

##### MC4 Connectors

![](https://raw.githubusercontent.com/solarworkshop/Small-Solar-Power-Systems-Zine/main/images/mc4.png)

Important: MC4 connectors are shaped different for positive and negative poles, make sure you know if you are connecting to a positive or negative wire before crimping on a connector.

TODO: how to tell positive and negative apart, when to use.

1. Assemble the components as shown above, sliding the screw on connector, outter cable ring, then gasket onto the wire.
2. Strip **¼ inch** of insulation from the wire.
3. Crimp an **MC4 metal pin** onto the wire using an **MC4 crimping tool**.
4. Insert the crimped pin into the MC4 plastic housing (male or female).
5. Push until it clicks, ensuring a secure connection.

- **For Bare Wire to Charge Controller (Screw Terminals):**

1. Strip roughly ½ inch of insulation or however much will fully go into the charge controller and leave none showing from the end of the wire.
2. Insert the bare wire into the charge controller terminal.
3. Tighten the screw securely.

**Safety Tips:  
Use an MC4 tool** to disconnect MC4 connectors—pulling by hand can damage them.  
**Check polarity (positive & negative)** before connecting to the charge controller.  
**Use a fuse or breaker** between the solar panel and charge controller for protection.

#### 2\. Connecting the Charge Controller to the Battery

**Wiring Type:** Battery cables usually connect via **ring terminals** or **spade terminals**, secured with bolts or screw terminals on the charge controller.

**How to Prepare the Wires:**

- **For Ring Terminals (Recommended for Battery Connections):**

TODO: explain 2 different types of ring terminals.

1. Strip **½ inch** of insulation from the end of the cable.
2. Slide a **heat-shrink ring terminal** onto the wire.
3. Crimp the terminal using a **heavy-duty crimper**.
4. Use a **heat gun or lighter** to shrink the insulation, sealing the connection.
5. Bolt the terminal onto the battery post.

![](https://raw.githubusercontent.com/solarworkshop/Small-Solar-Power-Systems-Zine/main/images/ring-terminal.jpg)

- **For Screw Terminals (Some Charge Controllers):**

1. Strip **½ inch** of insulation.
2. Insert the wire into the terminal.
3. Tighten the screw until the wire is securely held.

**Safety Tips:  
Always connect the battery to the charge controller BEFORE connecting solar panels.  
Use properly rated fuses** between the battery and charge controller.  
**Avoid over-tightening bolts**, which can damage terminals.

#### 3\. Connecting the Battery to the Inverter

**Wiring Type:** Large-gauge cables with **ring terminals**, secured to the battery and inverter using bolts.

**How to Prepare the Wires:**

1. Strip **½ inch to 1 inch** of insulation from the end of the cable.
2. Slide a **heat-shrink ring terminal** onto the wire.
3. Crimp it tightly using a **hydraulic crimper or hammer crimp tool**.
4. Use a **heat gun or lighter** to shrink the insulation over the connection.
5. Bolt the ring terminals onto the battery and inverter.

**Safety Tips:**

**Use properly sized cables** (too small = overheating).  
**Install a fuse close to the battery** on the positive wire.  
**Ensure ring terminals are tight but not over-tightened.**

#### 4\. Grounding a Solar System in a Vehicle

**Why Ground to a Vehicle?  
**Grounding the system to the vehicle’s chassis **helps prevent electrical faults** and provides a stable voltage reference.

**How to Ground the System:**

1. Find a **bare metal point** on the vehicle’s chassis (a factory grounding point is best).
2. Strip **½ inch** of insulation from the ground wire.
3. Crimp a **ring terminal** onto the wire.
4. Use a **heat gun or lighter** to shrink the insulation.
5. Secure the ring terminal to the chassis using a **bolt or self-tapping screw**.
6. Ensure the connection is **clean, tight, and free of paint or rust**.

![](https://raw.githubusercontent.com/solarworkshop/Small-Solar-Power-Systems-Zine/main/images/Car-Grounds.jpg)

**Safety Tips:  
Use the same gauge wire as the main battery cables** for grounding.  
**Avoid using small screws**—a solid bolt connection is best.  
**Check the connection regularly** for corrosion or looseness.

### Solar Panel Placement Considerations

Proper positioning of solar panels is **critical** for maximizing energy production. The angle, direction, and impact of shading all affect efficiency.

#### 1\. Solar Panel Positioning

**Direction (Azimuth Angle):**

- **In the Northern Hemisphere** → Face panels **South**
- **In the Southern Hemisphere** → Face panels **North**
- **If adjustable**, panels can be slightly turned **Southeast or Southwest** to optimize for morning or afternoon sun, depending on energy usage patterns.

#### 2\. Solar Panel Angle (Tilt) for Maximum Output

![](https://raw.githubusercontent.com/solarworkshop/Small-Solar-Power-Systems-Zine/main/images/pv-tilt.png)

The **tilt angle** should be adjusted based on latitude and seasons:

- **Fixed Angle (Year-Round Setup)**: **Tilt = Your Latitude** (e.g., for 35° latitude, set panels at 35° tilt).
- **Adjustable Angles for Seasonal Optimization**:
- **Summer:** **Latitude - 10°** (Panels lay flatter to capture higher sun).
- **Winter:** **Latitude + 10°** (Panels tilt more to capture lower sun).
- **Spring/Fall:** **Set to Latitude** (Balanced approach).
- **Vertical Mounting (90° Angle, Walls/Fences): Worst for solar production**, but useful in snowy areas to prevent snow buildup.

#### 3\. Effects of Shading on Solar Panels

**Shading is one of the biggest performance killers** in a solar system. Even a small amount of shade on one panel **can drastically reduce power output**, especially in **series-connected panels**.

#### Why Shading Reduces Power:

- **Partial shading can cause major losses.** If just **one cell** in a panel is shaded, it can reduce the entire panel’s output.
- **Series-connected panels suffer the most**—one shaded panel limits the entire string’s current.
- **Parallel-connected panels perform better**, since shading on one panel doesn’t affect others as much.

**How to Minimize Shading Issues:**

- **Avoid placing panels near trees, buildings, or antennas** that cast shadows.
- **Use bypass diodes** (built into many panels) to reduce shading impact.
- **Tilt panels properly** so shadows move quickly rather than lingering.

<!-- TOC --><a name="installation-longevity-considerations"></a>
# Installation Longevity Considerations

A well-organized **solar power system** is not only more **efficient and easier to maintain**, but it also ensures **safety and durability** in various environmental conditions. Below are best practices for **cable management, weather protection, and battery storage.**

### Keeping a Solar Installation Neat

![](https://raw.githubusercontent.com/solarworkshop/Small-Solar-Power-Systems-Zine/main/images/neat.jpg)

A messy install can lead to **power loss, troubleshooting difficulties, and safety risks.** Keep your system organized with these tips:

#### Cable Management Suggestions

- **Use proper wire sizes** to minimize voltage drop and prevent overheating.
- **Label all wires** (e.g., PV+, PV-, BAT+, BAT-) for easy identification.
- **Use conduit or cable raceways** to protect wires from physical damage.
- **Zip ties or cable clips** keep wiring bundles tidy and prevent them from moving in the wind.
- **Avoid sharp bends or tight loops** in cables to prevent stress on the wiring.

### Mounting Components Properly

- **Secure charge controllers, breakers, and inverters to a solid surface** (plywood board, metal bracket, or inside a weatherproof enclosure).
- **Leave enough space for ventilation**, especially around inverters and charge controllers that generate heat.
- **Use weatherproof junction boxes** for wire connections when installing outdoors.

### Protecting the System from the Elements

A solar installation is exposed to **sun, rain, wind, dust, and extreme temperatures**. Protecting components ensures longevity and reliability.

#### Solar Panels

- **Use strong mounts and brackets** rated for local wind speeds.
- **Ensure panels are tilted to allow water runoff** (prevents pooling and dirt buildup).
- **Use UV-resistant solar cables** to prevent deterioration over time.

#### Charge Controller & Inverter

- **Install indoors or in a weatherproof enclosure** to protect from rain and moisture.
- **If placed outside, use a NEMA-rated enclosure** (e.g., **NEMA 3R or NEMA 4X** for outdoor electrical protection).
- **Provide adequate airflow** around components to prevent overheating.

![](https://raw.githubusercontent.com/solarworkshop/Small-Solar-Power-Systems-Zine/main/images/outdoor-box.png)

#### Battery Bank

- **Keep batteries out of direct sunlight** and extreme heat to extend lifespan.
- **For flooded lead-acid batteries**, install in a ventilated space to release hydrogen gas safely.
- **Seal cable entry points** in battery enclosures to prevent dust and pests.

#### Consider a Battery Box

Proper battery storage is helpful for safety, ventilation, and temperature control.

##### Types of Battery Boxes:

**1\. DIY Wooden or Plywood Battery Box**

- Ideal for **indoor installations** (garage, shed, or RV).
- Allows **custom sizing** for multiple batteries.
- Must have **ventilation holes** for lead-acid batteries.
- Add **foam insulation** in cold climates to prevent freezing.

**2\. Plastic Marine-Grade Battery Box**

- Best for **single battery setups** (RV, boat, van).
- Resistant to **water, corrosion, and UV exposure**.
- Usually includes **tie-down straps** for secure mounting.
- Some models have **built-in vents** for gassing batteries.

<!-- TOC --><a name="alternative-ways-to-charge-batteries"></a>
# Alternative Ways to Charge Batteries

While solar is ideal, sometimes you’re only going out for a weekend and can do with a single battery charge from an AC wall charger ahead of time, and leave the panels at home (or build a system without them). If you are installing a solar setup (or standalone house battery) in a vehicle or RV you can charge your battery while driving using the power generated by your vehicles alternator.

### AC Wall Chargers

AC chargers are **plugged into a standard household outlet** (120V AC) and convert power to **12V DC** to charge a battery. You can purchase and use one of these to charge your batteries at home before you go on an outting where you need power.

#### Standard Battery Chargers

- Fast charging, good for deep-cycle batteries.
- Often rated at **10A-50A** output.
- Smart chargers can **prevent overcharging** by switching to trickle mode when full.

#### Trickle Chargers & Battery Maintainers

- Designed for **long-term maintenance** rather than fast charging.
- Typically **1A-3A output** to **slowly top off a battery**.
- Ideal for **seasonal vehicles (RVs, boats, motorcycles)** that sit unused.
- Many models **automatically shut off** or adjust current to prevent overcharging.

#### Smart Multi-Stage Chargers

- Uses **Bulk, Absorption, and Float** charging stages for optimal battery health.
- Works with **lead-acid, AGM, lithium, and gel** batteries.
- Prevents sulfation and extends battery life.

**Example Setup:**

- Plug charger into a **120V AC outlet**.
- Connect **positive (red) and negative (black) leads** to battery terminals.
- Set to the **correct battery type** (AGM, lithium, etc.).
- Monitor **charging progress**; most chargers have an LED or display showing charge percentage.

### Charging from a Vehicle Alternator

A vehicle’s **alternator** generates DC power while the engine runs, which can be used to charge **house batteries in an RV, camper, or off-grid setup**.

**What You Need:**

- Heavy-duty wiring (4 AWG - 8 AWG) to handle high currents

- Battery isolator or DC-DC charger** to prevent draining the starter battery

- Fuses or circuit breakers** to protect wiring

- Anderson connectors** or quick disconnects for easy removal

- Two Ways to Charge from an Alternator**

#### Using a Battery Isolator (Basic Setup):

- Allows alternator to charge a second battery while **keeping it separate from the vehicle’s starter battery**.
- Uses a **Voltage-Sensing Relay (VSR)** to connect batteries only when the engine is running.
- When the vehicle is off, the relay **disconnects** to prevent draining the starter battery.

**Basic Wiring:**

1. **Connect vehicle battery positive** to isolator input.
2. **Run heavy-duty wire** from isolator to house battery **(fused near both ends)**.
3. **Ground the system** properly to the vehicle’s chassis.

#### Using a DC-DC Charger (Better for Lithium & Deep-Cycle Batteries)

- A **DC-DC charger (20A-50A models)** ensures the house battery gets the correct charging voltage.
- Essential for **Lithium (LiFePO4) batteries**, since alternators don’t always reach their needed voltage.
- Provides **multi-stage charging** (Bulk, Absorption, Float).
- Protects the alternator from excessive load.

**Basic Wiring:**

1. Connect the vehicle’s alternator (via fuse) to the DC-DC charger input.
2. Connect the charger’s output to the house battery.
3. Ground both connections properly.
4. Mount the DC-DC charger near the battery for efficiency.

<!-- TOC --><a name="pv-panels-in-depth"></a>
# PV Panels In Depth

### Monocrystalline vs. Polycrystalline Solar Panels

Solar panels are commonly made using two types of silicon cells—**Monocrystalline** and **Polycrystalline**. Each has advantages and trade-offs:

| Feature                 | Monocrystalline                           | Polycrystalline                           |
|-------------------------|-------------------------------------------|--------------------------------------------|
| **Appearance**          | Uniform black cells with rounded corners  | Bluish cells with rectangular, speckled pattern |
| **Efficiency**          | Higher (15–23%)                           | Lower (13–17%)                             |
| **Space Efficiency**    | Higher—fewer panels for same output       | Lower—requires more panels                 |
| **Performance in Heat** | Slightly better in high temperatures      | Slightly worse in high temperatures        |
| **Cost**                | Higher initial cost                       | Lower initial cost                         |
| **Lifespan**            | Longer (~25–30+ years)                    | Shorter (~20–25 years)                     |

#### When to Use Monocrystalline
  - Ideal if your roof space is limited.
  - Maximizes efficiency and long-term reliability.
  - Better overall performance, especially in hotter climates.

> **Choose Monocrystalline** if you have limited space, need high efficiency, and prioritize long-term reliability.  

#### When to Use Polycrystalline
  - Best choice if budget is the main concern.
  - Good if you have plenty of available installation space.
  - Practical for larger arrays where cost matters more than peak efficiency.

> **Choose Polycrystalline** if budget is your primary concern and you have plenty of installation space.

### Testing PV Panels & Understanding Their Labels

It's important to test the voltage and amperage of your solar panels to ensure they are still functional and operating close to their rated specifications. You can also learn a lot from reading the label on the back of the panel.

#### How to Read a Solar Panel Label

Most solar panels have a label on the back that provides **electrical specifications**. Here’s how to interpret key values:

| **Label Term** | **What It Means** | **Typical Values (Example for a 100W Panel)** |
| --- | --- | --- |
| **Max Power (Pmax)** | The maximum wattage output under ideal conditions. | **100W** |
| **Voltage at Max Power (Vmp)** | The voltage the panel produces under load (when connected to a system). | **18V - 20V** |
| **Current at Max Power (Imp)** | The current (amps) the panel produces under load. | **5A - 6A** |
| **Open Circuit Voltage (Voc)** | The voltage when the panel is not connected to anything (no load). | **22V - 24V** |
| **Short Circuit Current (Isc)** | The maximum current the panel can produce when shorted. | **5.5A - 6.5A** |
| **Operating Voltage Range** | The panel’s recommended working range. | **12V (nominal) or 24V (nominal)** |

🔹 **Important Notes:**

- **Vmp is the actual working voltage**, while **Voc is higher and occurs when the panel is disconnected**.
- **Imp is the working current**, while **Isc is the max current when shorted**.
- **If a used panel’s actual output is significantly lower than these values, it may be damaged**.

#### How to Test a Used Solar Panel

##### **A. Testing Open Circuit Voltage (Voc) with a Multimeter**

**What it tells you:** If the panel is still producing power and if there’s damage to internal connections.

**Steps:**

1. Place the panel in **full sunlight** (angle it towards the sun for max exposure).
2. Set your **multimeter to DC voltage (VDC)**.
3. Connect the **positive probe to the positive MC4 connector** (or junction box terminal).Connect the **negative probe to the negative connector**.
4. Compare the reading to the **Voc value on the label**.

**Good result:** A reading **close to Voc** (e.g., if Voc is 22V, you should measure around 20V-22V in full sun).  
**Bad result:** If the voltage is **significantly lower** (e.g., under 15V for a 22V Voc panel), the panel may have **bad cells or internal damage**.

##### **B. Testing Short Circuit Current (Isc) with a Multimeter**

**What it tells you:** If the panel is capable of producing its maximum rated current.

**Steps:**

1. Set your **multimeter to DC amps (A or mA mode)**.
2. Place the panel in **full sunlight**.
3. Connect the **positive probe to the positive panel wire**.
4. Connect the **negative probe to the negative panel wire**.
5. Compare the reading to the **Isc value on the label**.

**Good result:** A reading **close to Isc** (e.g., if Isc is 5.5A, you should see around 5A-5.5A).  
**Bad result:** If the current is much lower, **some cells may be failing, or there is shading/damage**.

**Warning:** Some multimeters can only handle small currents (e.g., 10A max). If the panel exceeds this, use a **clamp meter** or a proper charge controller test instead.

**Good result:** Output **at least 70-80% of rated power** under good sunlight.  
**Bad result:** If power is much lower than expected, the panel has **cell degradation, dirt, or internal failure**.

#### **Troubleshooting Low Solar Panel Output**

- **Check for Shading** – Even a small amount of shade **drastically reduces power output**.
- **Inspect for Cracks or Delamination** – Damaged panels often underperform.
- **Clean the Panel** – Dirt, dust, or oxidation can block sunlight and reduce efficiency.
- **Check for Loose Connections** – Bad MC4 connectors or wiring can cause voltage drops.
- **Measure Temperature** – **Hot panels produce less power** than their rated values.

<!-- TOC --><a name="charge-controllers-in-depth"></a>
# Charge Controllers In Depth

### Why Do You Need a Solar Charge Controller?

Solar panels often produce voltages higher than what batteries safely accept, especially in direct sunlight or cold temperatures. A charge controller adjusts this voltage and current, preventing battery damage and extending battery lifespan.

### PWM vs. MPPT Charge Controllers

There are two main types of charge controllers: **PWM** (Pulse Width Modulation) and **MPPT** (Maximum Power Point Tracking).  
While both do the same basic job, they work very differently and are suited to different types of systems.

#### PWM (Pulse Width Modulation) Charge Controllers

- **How It Works**:  
  A PWM controller connects the solar panel directly to the battery when charging. As the battery charges up, the controller rapidly "pulses" the connection on and off to maintain the correct voltage without overcharging.
  
- **Voltage Matching**:  
  The solar panel’s voltage is pulled down to match the battery’s voltage. This means if you have a 12V battery, the panel’s voltage must also be around 12V to work efficiently.

- **Efficiency**:  
  Generally about **70–80% efficient**, because it doesn’t make full use of higher panel voltages.

- **Best For**: Smaller systems; when panel voltage is close to battery voltage; lower-cost, budget setups.

- **Pros**: Inexpensive; simple and reliable; great for small DIY systems.
  
- **Cons**: Wastes potential power if panel voltage is much higher than battery voltage; less efficient in cold or cloudy weather

#### MPPT (Maximum Power Point Tracking) Charge Controllers

- **How It Works**:  
  An MPPT controller is more sophisticated. It constantly measures the output of the panels and finds the **maximum power point** — the optimal combination of voltage and current to produce the most power.  
  It then **converts** that higher voltage down to match the battery voltage, while **boosting the current** to deliver more charging power.

- **Voltage Flexibility**:  
  MPPT allows you to use solar panels with a much higher voltage than your battery bank. For example, you can use a 36V or 48V panel to charge a 12V battery.

- **Efficiency**:  
  Typically **90–99% efficient**, especially in cold or cloudy conditions when panel voltage tends to be higher.

- **Best For**: Larger systems; situations where panel voltage is significantly higher than battery voltage; cold climates (where panels can generate extra voltage); systems where you want to maximize every bit of solar power.

- **Pros**: Much more efficient, especially with high-voltage panels; allows longer wiring runs (because higher voltage travels better over distance); better performance in changing weather.

- **Cons**: More expensive; slightly more complex electronics (but still very reliable).

#### Summary Table

| Feature | PWM Controller | MPPT Controller |
|:--------|:---------------|:----------------|
| **Efficiency** | 70–80% | 90–99% |
| **Cost** | Low | Higher |
| **Best Use** | Small, simple systems | Larger, high-performance systems |
| **Panel-to-Battery Voltage** | Must be matched closely | Panel voltage can be much higher |
| **Performance in Cold/Cloudy Weather** | Lower | Much better |

#### Quick Example

Suppose you have a 200W solar panel rated at 18V and a 12V battery:
- A **PWM controller** would force the panel down to 12V, wasting the difference in voltage.
- An **MPPT controller** would keep using the full 18V, converting it efficiently to deliver more amps into your battery — meaning you get almost the full 200W available.

### Other Charge Controller Considerations

#### Voltage and Current Ratings
- Ensure your charge controller matches your battery bank’s voltage (12V, 24V, or 48V).
- Check the maximum current rating (amps) to accommodate your solar panels’ combined current output.

#### Battery Compatibility
- Make sure the controller supports your battery chemistry (lead-acid, AGM, lithium).
- Many controllers offer customizable charging profiles for different battery types.

#### Load Control & Low Voltage Disconnect (LVD)
- Many controllers have terminals to power DC loads directly, automatically disconnecting them if the battery voltage gets too low.

#### Temperature Compensation
- Adjusts charging voltage according to battery temperature, prolonging battery life.
- Important for lead-acid and AGM batteries in climates with large temperature variations.

#### Remote Monitoring and Display
- LCD screens, smartphone apps, or computer interfaces help you track system performance easily.

### Proper Sizing of a Charge Controller

Follow these steps to choose the right size controller:

1. **Calculate Total Solar Panel Current (Amps)**  
   Example: Four panels at 5 amps each = **20 amps** total.

2. **Add a 25% Safety Margin**  
   Example: 20A × 1.25 = **25 amps**.  
   Choose at least a 30-amp controller.

3. **Confirm Voltage Compatibility**  
   Match battery bank and controller voltage (12V, 24V, or 48V).


### Installation & Safety Tips

- Mount your controller close to your battery bank to minimize voltage drop.
- Always use proper fuses or circuit breakers between panels, controller, and batteries.
- Ensure proper ventilation around the controller to prevent overheating.
- Regularly inspect connections and terminals for corrosion, dirt, or looseness.

#### Common Mistakes to Avoid

- Using a PWM controller with high-voltage panels, causing efficiency losses.
- Overloading your charge controller by exceeding its rated amps.
- Ignoring proper battery type settings, leading to battery damage.
- Mounting the charge controller in enclosed areas with no airflow.

<!-- TOC --><a name="batteries-in-depth"></a>
# Batteries In Depth

### Understanding Battery Measurements

Batteries are the heart of a small solar power system. Knowing how to read and understand their ratings is critical for designing, using, and maintaining your system properly. Here are the key measurements and what they mean:

#### **Depth of Discharge (DoD)**
- How much energy you can use before needing to recharge.
- Lead-acid batteries recommend 50% DoD; lithium batteries allow 80–90% DoD safely.

#### **State of Charge (SoC)**
- How full a battery is at any moment, usually shown as a percentage.

#### **C-Rate**
- How fast you can charge or discharge a battery relative to its total capacity.
- Example: 1C = full discharge in 1 hour; 0.5C = full discharge in 2 hours.

#### **Cycle Life**
- The number of complete charge/discharge cycles a battery can undergo before its capacity significantly declines.

#### **Voltage**
- Common battery system voltages: 12V, 24V, and 48V.
- Higher voltage systems (24V/48V) are more efficient for larger solar arrays and inverters.

### Battery Chemistries

### Lead-Acid Batteries (Flooded, AGM, and Gel)**

#### Flooded Lead-Acid (FLA):

- Cheapest, but requires **maintenance (adding water) and ventilation**.
- Lifespan: **3-5 years** (if well-maintained).
- Depth of Discharge (DoD) should stay **above 50%** for longevity.

#### Absorbed Glass Mat (AGM):

- Maintenance-free and spill-proof.
- Better lifespan than FLA (**4-7 years**).
- Can handle higher charge/discharge rates.

#### Gel Batteries:

- Similar to AGM but **slower charging** and more sensitive to overcharging.
- Not ideal for high-current applications.

**Best For:** Budget systems, low-maintenance setups, backup power.

**Downsides:** Heavy, shorter lifespan, lower efficiency than lithium.

#### Lithium Iron Phosphate (LiFePO4)

- **Most efficient battery type (~95% charge efficiency).**
- **Can be discharged to 80-90% DoD** without damage.
- **Lasts 10-15 years** (3000-6000 cycles).
- No ventilation needed, lightweight, handles high charge/discharge rates.

**Best For:** Long-term solar storage, high performance, low maintenance.

**Downsides:** Higher upfront cost, **requires a BMS (Battery Management System)**.

#### Common Types of Solar Batteries Summary

| Battery Type | Pros | Cons | Typical Use |
|--------------|------|------|-------------|
| **Flooded Lead-Acid (FLA)** | Cheapest upfront; well understood | High maintenance (must add water); shorter lifespan; vent hydrogen gas | Budget systems; off-grid cabins |
| **Sealed Lead-Acid (AGM, Gel)** | Maintenance-free; spill-proof; simple charging | Heavier; less deep cycling ability; moderate lifespan | Small to medium systems; backup setups |
| **Lithium-Ion (LiFePO4)** | Long lifespan (3000–5000+ cycles); high efficiency; lightweight; no maintenance | High upfront cost | Medium to large off-grid systems; mobile setups (vans, RVs) |
| **Nickel-Based (NiMH, NiCd)** | Durable in extreme conditions; long cycle life | Expensive; less efficient; specialized use cases | Harsh climates; industrial setups |

### Temperature Effects on Battery Performance

| **Battery Type** | **Cold Weather Performance (< 0°C / 32°F)** | **Hot Weather Performance (> 30°C / 86°F)** |
| --- | --- | --- |
| **Flooded Lead-Acid** | Reduced capacity, thickens electrolyte, harder to charge | Increased water loss, shorter lifespan |
| **AGM / Gel** | Slightly better than FLA, but still reduced | Heat causes plate degradation |
| **Lithium (LiFePO4)** | !! Cannot charge below 0°C without a heater | Performs well, but heat shortens lifespan |

- **In Cold Weather:** Lithium must be **above freezing to charge**. Some models have built-in heaters.
- **In Hot Weather:** High temperatures cause **faster aging** in all battery types. Store batteries in shaded, ventilated areas.

### Battery Charge Profiles & Charge Curves

Each battery type follows a **specific charge curve** to optimize lifespan and performance. The charge profile describes the different phases of the battery charging, when and how long each of these phases happens, and the voltage applied for each.

It is important to know the charge profile for the type of battery that you're using and make sure any method you are using to charge it (solar charge controller, wall / trickle charger, vehicle alternator) is compatible with and or set to the charge profile of your specific battery. It is also important to know what voltage to apply to your battery. Failing to do either of these can result in a lessening of the life of your battery or rendering it useless after a small number of charge cycles.

Most charge controllers will have presets for common battery chemistries that you can enable, and usualy off the shelf they default to AGM. If you find yourself with a charge controller that does not allow you to set the battery type and you don't know what type of battery it is programmed for, be wary of connecting it to any batter you don't want to damage. More advanced charge controllers will allow you to fine tune these presets. This is a larger topic that is worth researching if you've invested a lot of money in batteries and want them to last as long as possible.

Here is a little bit about common battery chemistries and their charging profiles:

#### Lead-Acid Charging Stages

1. **Bulk Charge (Fastest Stage)** → Charger delivers **constant current** until ~80% full.
2. **Absorption Charge** → Voltage **stabilizes**, current tapers off.
3. **Float Charge** → Maintains full charge without overcharging.

**Typical Voltage Ranges:**

- 12V Flooded: **14.4V (Absorption), 13.6V (Float)**
- 12V AGM/Gel: **14.2V (Absorption), 13.8V (Float)**

#### Lithium Charging Stages

1. **Bulk Charge** → Rapid charging at **constant current** until ~99% full.
2. **Taper Off** → Once full, charge current drops, but **no trickle charging needed**.

**Typical Voltage Range:**

- 12V LiFePO4: **14.2V - 14.6V full charge, 13.3V resting voltage**

**Important:** Lithium **does not need float charging**—overcharging shortens lifespan.

### Battery Features to Consider

#### Battery Chemistry
- Choose based on budget, maintenance tolerance, desired lifespan, and system needs.

#### Capacity (Amp-Hours and Kilowatt-Hours)
- **Amp-Hours (Ah)** measure storage at a given voltage.
- **Kilowatt-Hours (kWh)** measure total energy storage.
- Formula: **kWh = (Ah × V) ÷ 1000**

#### Physical Size and Weight
- Lead-acid batteries are heavy; lithium batteries are lighter for the same capacity.
- Ensure your structure or vehicle can handle the weight.

#### Temperature Tolerance
- Batteries degrade faster when exposed to extreme heat or cold.
- Lithium batteries often have built-in protection but can’t be charged below freezing without special heaters.

#### Maintenance Requirements
- Flooded lead-acid batteries require regular watering and cleaning.
- AGM, Gel, and Lithium batteries are maintenance-free.


### Proper Battery Sizing

Steps to size your battery bank:

1. **Calculate your daily energy use (Wh or kWh)**.
2. **Multiply by days of storage needed** (e.g., 2-3 days of backup).
3. **Factor in DoD** (e.g., use only 50% of lead-acid battery capacity).
4. **Account for inefficiencies** (about 10–15%).

**Example:**
- Daily use = 1000Wh
- 2 days of backup = 2000Wh
- Lead-acid battery @ 50% DoD → need 4000Wh of storage
- 12V system: 4000Wh ÷ 12V = ~333Ah battery bank needed.

### Installation and Safety Tips

- Always use proper fusing between batteries and other system components.
- Secure batteries to prevent movement or tipping.
- Ensure ventilation if using flooded lead-acid batteries (they release hydrogen gas when charging).
- Avoid exposing batteries to extreme temperatures if possible.

### Common Mistakes to Avoid

- Using starter (automotive) batteries instead of deep-cycle batteries.
- Undersizing your battery bank, leading to frequent deep discharges and short lifespan.
- Mixing old and new batteries, or different brands/capacities, in one bank.
- Ignoring ventilation needs for lead-acid batteries.


<!-- TOC --><a name="inverters-in-depth"></a>
# Inverters In Depth

### Features to Consider

#### **Output Power Rating (Watts)**
- **Continuous Wattage**: The amount of power the inverter can provide continuously. 
- **Surge Wattage**: Higher temporary output to handle startup loads of appliances (like fridges, motors, or pumps).

#### **Input Voltage**
- Must match your battery system voltage (12V, 24V, or 48V).

#### **Efficiency**
- Higher efficiency inverters waste less energy as heat, reducing power loss. Look for efficiency ratings of 85–95% or higher.

#### **Built-In Safety Features**
- Automatic shutdown on overload or overheating.
- Built-in fuses or circuit breakers for safety.
- Short-circuit protection to prevent damage.

#### **Remote Monitoring & Control**
- Some modern inverters come with remote control or monitoring features, such as Bluetooth, Wi-Fi, or remote panels for easy management.

#### **Noise Levels**
- Inverters with cooling fans can be noisy; consider fanless designs or quieter models if this matters for your application.

### Proper Sizing of an Inverter

Choosing the right size inverter depends on your load requirements:

1. **List all the devices** you plan to power simultaneously.
2. **Calculate total continuous wattage** needed (sum up all devices).
3. **Add 25–50% buffer** to account for surge loads and future expansion.

For example:

| Device                 | Continuous Watts | Surge Watts |
|------------------------|------------------|-------------|
| Refrigerator           | 150W             | 800W        |
| LED Lights (3 × 10W)   | 30W              | 30W         |
| Laptop                 | 60W              | 60W         |
| **Total**              | **240W**         | **890W**    |

In this example, choose an inverter rated at least 500W continuous and ~1000W surge capacity.

### Pure vs. Modified Sine Wave Inverters

Inverters are a key part of many solar power systems. They **convert DC electricity** from your batteries into **AC electricity** that your home appliances can use.  
There are two main types of inverters based on the kind of AC wave they produce: **Pure Sine Wave** and **Modified Sine Wave**.

#### Pure Sine Wave Inverters

- **Produces clean, smooth power** that closely matches the electricity from the utility grid.
- **Safe for all electronics**, including sensitive devices like laptops; medical equipment; newer refrigerators; LED TVs; microwaves.
- **Most efficient and safest option** for running all types of appliances.

**Pros**: Compatible with all devices; runs equipment cooler and quieter; reduces risk of damaging sensitive electronics.  
**Cons**: More expensive than modified sine wave inverters.

#### Modified Sine Wave Inverters

- **Produces a rough, choppy power output** — not a smooth wave.
- Works fine for **simple tools and appliances** like power drills; older TVs; some lights; simple pumps and motors.
- Can cause problems with sensitive electronics: noisy operation (buzzing sounds); lower efficiency; potential overheating or damage to some devices.

**Pros**: Much cheaper; good for simple, rugged applications.  
**Cons**: May not run all electronics properly; can shorten the lifespan of certain devices.

#### Which Inverter Should You Buy?

- **If you plan to run sensitive electronics** (laptops, TVs, refrigerators, CPAP machines, etc.):  
  ➔ **Buy a Pure Sine Wave inverter**.

- **If you're only running simple tools or resistive loads** (older appliances, basic lighting, pumps, etc.) and want to save money:  
  ➔ **A Modified Sine Wave inverter may be enough**, but know the risks.

- **General Advice**:  
  If you can afford it, **choose a Pure Sine Wave inverter**.  
  It provides better performance, more flexibility, and protects your equipment.

<!-- TOC --><a name="design-and-wire-a-12v-fuse-box"></a>
# Design and Wire a 12V Fuse Box

Using 12V DC devices in a solar setup is usually more efficient because you avoid the energy losses that happen when using an inverter to convert to 120V AC. It also makes the system simpler, cheaper, and safer to install. If all your devices can run on 12V, you’ll save power and reduce system complexity — but you’ll still need an inverter if you want to run regular household appliances.

A **12V fuse box** is essential for distributing power safely to multiple 12V loads (lights, fans, USB chargers, etc.) in a solar system. It prevents **overloads, short circuits, and fire hazards** by using appropriately rated fuses for each circuit.

#### 1\. Choosing a 12V Fuse Box

**Types of Fuse Boxes:**

- **Blade-Style Fuse Block:** Uses standard automotive **ATO/ATC fuses** (most common).
- **Glass Fuse Panel:** Uses cylindrical glass fuses (less common, mostly in older setups).
- **Inline Fuse Holders:** Used for single circuits rather than a full panel.

**What to Look For:  
Number of Circuits:** Choose a fuse box with enough slots for all your 12V loads (usually 4-12 circuits).  
**Common or Independent Positive Bus Bar:** A common bus bar lets you connect all circuits to one power source.  
**Ground Bus Bar (Optional):** Some fuse blocks include a ground bus, which simplifies wiring.  
**Cover:** Protects fuses from dust, moisture, and accidental contact.

#### 2\. Choosing the Right Wire Gauge & Fuse Sizes

**Wire size depends on the current (amps) each circuit draws.** The fuse should be **slightly larger** than the load’s operating current but never exceed the wire’s capacity.

See the fuse and wire size sections above for me details.

#### 3\. Wiring the 12V Fuse Box

**Components Needed:**

- **12V Fuse Box** (with slots for fuses)
- **Appropriate Fuses** (based on your load)
- **Main Power Cable (Positive & Negative Wires)**
- **Ring Terminals** (for secure connections)
- **Crimping Tool & Heat Shrink**

### **Step-by-Step Wiring**

#### **A. Connecting the Main Power Wires**

1. **Run a wire from the battery's positive terminal** (through a fuse or breaker) to the **input terminal** of the fuse box.
    1. **Use a 6-10 AWG wire** depending on total load.
    2. **Install a main fuse (30A-100A) close to the battery.**
2. **Connect the fuse box’s negative bus bar (if available) to the battery’s negative terminal** using a properly sized wire.
3. If no negative bus bar exists, connect all device negatives to the battery’s negative post or vehicle chassis.

#### **B. Wiring Individual Circuits**

1. **Strip the wire ends** (~½ inch) for each 12V device.
2. **Crimp ring terminals or spade connectors** onto the wire ends.
3. **Insert each wire into the appropriate fuse slot**, ensuring:
    1. The **positive wire** from each device connects to a **fused terminal**.
    2. The **negative wire** connects to the fuse box’s **ground bus bar** or directly to the battery/chassis ground.
4. **Insert the correct fuse** for each circuit.

#### **C. Protecting & Organizing the Wires**

1. **Use cable ties** to bundle wires neatly.
2. **Label each circuit** to easily identify which fuse controls each device.
3. **Secure the fuse box** in a dry, accessible location.

#### **4\. Safety & Best Practices**

- **Use a main fuse (30A-100A) between the battery and the fuse box.**
- **Avoid long wire runs** to minimize voltage drop (keep wires as short as possible).
- **Do not exceed the wire’s amp rating**—if in doubt, use a larger gauge.
- **Test each circuit** with a multimeter after wiring to ensure proper voltage.

#### **Wiring Diagram**

\[ 12V Battery \] ---- (Main Fuse) ---- \[ Fuse Box \] ---- (Fused Circuits) ---- \[ Loads \]

Each **fused circuit** powers a **12V device**, and all negatives return to the **battery negative or chassis ground**

<!-- TOC --><a name="considerations-for-bigger-than-12v-systems"></a>
# **Considerations for Bigger (than 12V) Systems**

While **12V solar systems** are common for small setups like RVs, boats, and off-grid cabins, **24V, 48V, and higher-voltage systems** offer advantages for larger power needs. Choosing the right voltage depends on **power requirements, wire sizing, and component compatibility**.

### **1\. Advantages & Disadvantages of Different System Voltages**

| **System Voltage** | **Best For** | **Advantages** | **Disadvantages** |
| --- | --- | --- | --- |
| **12V** | Small systems (under ~1500W), RVs, boats, DIY off-grid | Common, compatible with 12V appliances, cheaper controllers & inverters | Higher wire losses, inefficient for large loads |
| **24V** | Medium-sized systems (~1500W–5000W), cabins, workshops | Less voltage drop, thinner wires needed, more efficient than 12V | Fewer direct 24V appliances, may need a DC-DC converter |
| **48V** | Large off-grid homes, backup power, industrial | Best efficiency, minimal wire loss, supports high-power inverters | Requires 48V-compatible equipment, higher initial cost |

**General Rule:** **Higher voltage = less current = lower wire losses**.

### **2\. Wire Sizing & Voltage Drop Considerations**

- **Higher-voltage systems (24V, 48V) allow thinner wires** because **current (amps) is lower** for the same power output.
- Example:
- **12V @ 1000W → ~83A (large wires needed)**
- **24V @ 1000W → ~42A (smaller wires)**
- **48V @ 1000W → ~21A (even smaller wires)**

If using **longer cable runs**, higher voltages reduce losses and improve efficiency.

### **3\. Solar Panel Configuration for Higher Voltage Systems**

#### **A. 12V System**

- Uses **12V panels (nominal 18V Vmp) in parallel** for higher current.
- Panels stay **parallel** to keep voltage at 12V.

#### **B. 24V System**

- Uses **two 12V panels in series** (or native 24V panels).
- Keeps current lower while doubling voltage.

#### **C. 48V System**

- Uses **four 12V panels in series** (or native 48V panels).
- Ideal for reducing wire size and losses.

**Important:** Charge controllers (MPPT or PWM) must match the **battery bank voltage**.

### **4\. Battery Bank Considerations**

- **12V Systems** → Single **12V batteries** in parallel for more capacity.
- **24V Systems** → Two **12V batteries in series** (or 24V batteries).
- **48V Systems** → Four **12V batteries in series** (or 48V battery banks).

**Series connections increase voltage** without adding extra current.  
**Parallel connections increase capacity (Ah)** but keep the voltage the same.

!!! **Battery Chargers & Inverters Must Match Battery Voltage** – A 12V inverter **won't work** on a 24V system!

### **5\. Charge Controllers & Inverters for Different Voltages**

**PWM Controllers:** Only efficient if solar panel voltage closely matches battery voltage. Best for small 12V setups.  
**MPPT Controllers:** Can step down higher panel voltages (e.g., 100V solar array to 24V or 48V battery). Best for **24V+ systems**.

**Inverters:** Must match battery bank voltage (12V, 24V, 48V models available).

**DC-DC Converters:** Used to step down voltage for **12V accessories** in a 24V or 48V system.

### **6\. Safety & Regulations for Higher Voltages**

- **48V+ systems are considered "high voltage"** and require proper insulation and safety precautions.
- **Fuses & breakers** must be rated for the system voltage and installed at each major component.
- **Disconnect switches** should be used for maintenance and safety.

**Warning:** DC voltage is more dangerous than AC at high levels—use proper safety gear when working with **48V+ systems**.

<!-- TOC --><a name="tools-connectors-and-other-hardware"></a>
# **Tools, Connectors, and Other Hardware**

A proper solar installation requires a variety of **tools for wiring, mounting, and securing components**, as well as **specialized connectors and crimpers** for making reliable electrical connections. Here are most of the tools and components you'll want to have on hand for a sucessful solar project:

## **A. Electrical Tools**

**Wire Cutters** – For cutting battery cables, solar wires, and general wiring.  
**Wire Strippers** – To remove insulation from cables before crimping.  
**MC4 Crimping Tool** – For making professional MC4 solar connections.  
**Cable Lug Crimper (Hydraulic or Manual)** – Used for crimping battery lugs (6 AWG and larger).  
**Multimeter** – Essential for checking voltage, continuity, and resistance.  
**Clamp Meter (DC Capable)** – Measures current without breaking a circuit.  
**Heat Gun or Lighter** – For heat-shrink tubing on cable connections.
**Electrical Tape** - You never know when you’ll need it.  
**Fuse Puller** – Makes replacing fuses easier and safer.
**Box Cutter** - Sometimes useful to strip thick wires.
**Soldering Iron** - To make more secure connections or join multiple wires.

## **B. Mounting & Structural Tools**

**Drill & Drill Bits** – For mounting brackets, charge controllers, and junction boxes.  
**Screwdrivers (Flathead & Phillips)** – For securing terminal blocks and electrical components.  
**Wrenches & Ratchet Set** – For tightening nuts and bolts on racking and battery terminals.  
**Zip Ties & Wire Looms** – For organizing and securing wiring.

## **2\. Connectors & Wiring Components**

### **A. Solar Panel Connectors & Wiring**

**MC4 Connectors** – Standard **weatherproof** connectors for solar panels.  
**MC4 Y-Branch Splitters** – Used for parallel panel connections.  
**Solar Extension Cables (10 AWG - 12 AWG)** – Pre-terminated solar cables for easy connections.  
**Solar Combiner Box** – Organizes multiple solar strings before connecting to a charge controller.

### **B. Battery & Inverter Connections**

**Copper Battery Lugs (2 AWG - 8 AWG)** – For secure battery and inverter connections.  
**Heat Shrink Tubing** – Provides insulation and strain relief on lug connections.  
**ANL or MIDI Fuse Holders & Fuses** – Protects battery wiring and inverter circuits.  
**Bus Bars** – Distributes power between batteries and system components.  
**Battery Terminal Covers** – Prevents accidental short circuits.

### **C. Charge Controller & DC Distribution**

**Inline Fuse Holders (ATC or ANL)** – Protects charge controller wiring.  
**DC Circuit Breakers (Rated for 12V, 24V, 48V Systems)** – Provides resettable overcurrent protection.  
**Anderson Powerpole Connectors** – Useful for quick-disconnect battery or accessory connections.

## **3\. Recommended Crimpers**

**MC4 Crimping Tool** – Required for making custom solar cable connections  

**Hydraulic Lug Crimper (10 AWG - 4/0 AWG)** – Best for large battery cables.  
**Ratchet Wire Crimper (10-22 AWG)** – For smaller wiring connections (fuses, relays, etc.).  
**Anderson Powerpole Crimper** – If using Powerpole connectors for accessories.

### Solar Repair Go Kit

If you're not building a system from scratch but want to have the essentials on hand, we recommend at bare minimum packing these items:

- Multimeter
- Wire strippers
- Wire cutters
- Box cutter
- Medium size flat head and phillips screw driver
- Electrical tape
- Extra fuses
- Some lengths of 10 AWG wire and 14 or 16 AWG wire


Any of the smaller items in the bigger list above wouldn't hurt to have too if they fit in your bag.

### Battery Powered Soldering Irons

Battery powered soldering irons are relativley cheap, and if you find yourself regularly doing eletrical repairs in the field, carrying an iron and other soldering essentials can be a game changer.

There are cheap (around \$30) soldering irons you can find online that will fit batteries from common widely used power tool brands, which is very handy.

<!-- TOC --><a name="12v-solar-systems-budget-examples"></a>
# 12V Solar Systems Budget Examples

### **1\. Very Small 12V System (~$150 - $300)**

**Shopping List:**

**Solar Panel:** 50W-100W ($50 - $100)

**Charge Controller:** 10A PWM ($15 - $30)

**Battery:**

- **Sealed Lead Acid (SLA):** 12V 35Ah-50Ah ($60 - $120)
- **AGM:** 12V 35Ah-50Ah ($75 - $150)

**Inverter (Optional):** 150W-300W ($25 - $50)

**Wiring & Mounting Kit:** ($20 - $40)

**Total Cost:** **$150 - $300**

### **2\. Small 12V System (~$350 - $500)**

**Shopping List:**

**Solar Panel:** 100W-200W ($100 - $200)

**Charge Controller:** 20A PWM or small MPPT ($30 - $80)

**Battery:**

- **Sealed Lead Acid (SLA):** 12V 50Ah-100Ah ($100 - $200)
- **AGM:** 12V 50Ah-100Ah ($150 - $300)
- **LiFePO4:** 12V 50Ah ($220 - $280)

**Inverter:** 300W-500W ($50 - $80)

**Wiring & Accessories:** ($30 - $50)

**Total Cost:** **$350 - $500**

### **3\. Medium 12V System (~$500 - $650)**

**Shopping List:**

**Solar Panel:** 200W-300W ($200 - $250)

**Charge Controller:** 30A MPPT ($80 - $120)

**Battery:**

- **Sealed Lead Acid (SLA):** 12V 100Ah ($150 - $250)
- **AGM:** 12V 100Ah ($200 - $300)
- **LiFePO4:** 12V 100Ah ($280 - $350)

**Inverter:** 500W-1000W Pure Sine Wave ($80 - $120)

**Wiring & Accessories:** ($50 - $70)

**Total Cost:** **$500 - $650**

### **4\. Medium 12V System 2 (~$650 - $750)**

**Shopping List:**

**Solar Panel:** 300W-400W ($250 - $350)

**Charge Controller:** 40A MPPT ($100 - $140)

**Battery:**

- **Sealed Lead Acid (SLA):** 12V 100Ah-150Ah ($180 - $300)
- **AGM:** 12V 100Ah-150Ah ($200 - $300)
- **LiFePO4:** 12V 100Ah ($280 - $350)

**Inverter:** 1,000W Pure Sine Wave ($120 - $160)

**Wiring & Accessories:** ($80 - $100)

**Total Cost:** **$650 - $750**

### **Battery Type Cost Comparison**

| **Battery Type** | **Capacity** | **Typical Cost** | **Best Use Case** | **Lifespan (Cycles)** |
| --- | --- | --- | --- | --- |
| **Sealed Lead Acid (SLA)** | 35Ah-150Ah | $60 - $300 | Budget setups, backup power | ~300-500 cycles |
| **AGM (Absorbed Glass Mat)** | 50Ah-150Ah | $75 - $300 | Moderate use, no maintenance | ~500-800 cycles |
| **LiFePO4 (Lithium Iron Phosphate)** | 50Ah-100Ah | $220 - $350 | Long-term off-grid, lightweight | ~2000-5000 cycles |

<!-- TOC --><a name="beginner-solar-system-planning-checklist"></a>
# Beginner Solar System Planning Checklist

### Solar Panels

- Are they the appropriate voltage for your system, especially if you're using a PWM charge controller?
- Is the combined amperage lower than your charge controller’s input rating?
- Do you know where and how you are mounting them (roof, ground, pole, rack)?
- Do you have a spot that gets enough direct sun for most of the day?
- If using multiple panels, are you wiring them in series, parallel, or series-parallel to achieve the desired voltage and amperage?
- What size and type of wire do you need to connect them to the charge controller (consider voltage drop)?
- Have you tested the panels with a multimeter before connecting them?
- Do you have proper fusing or a breaker between the panels and the charge controller?

### Charge Controller

- Do you know if your charge controller is PWM or MPPT?
- Do you know how to set or change the battery type and charging profile (AGM, lithium, flooded, etc.)?
- Is your charge controller rated for the total voltage and current coming from the solar panels?
- Do you have a place to mount the controller with adequate ventilation (not in a sealed box)?
- Have you planned appropriate wire size between charge controller and battery bank?
- Are you using a fuse or circuit breaker between the controller and the battery?

### Battery

- Do you know the battery chemistry (lead-acid, AGM, lithium, etc.)?
- Do you understand the recommended Depth of Discharge (DoD) for your battery type?
- Is the battery sized properly for your expected daily power use and backup needs?
- Do you know the proper charging voltage settings for your battery chemistry?
- Do you have a safe place to install the battery (dry, ventilated, out of extreme heat or cold)?
- Are you protecting the battery bank with fuses or breakers?
- Are your batteries secured against tipping, sliding, or vibration?

### Inverter (if using one)

- Is the inverter rated for the maximum load you expect to run?
- Is it a Pure Sine Wave inverter if you plan to run sensitive electronics?
- Have you sized the wire and fuse properly between the battery and inverter?
- Do you have a manual shutoff switch for the inverter for safety?

### Wire Sizing and Protection

- Have you calculated the correct wire size for each part of the system based on current (amps) and distance (voltage drop)?
- Are you using stranded wire (not solid) for DC circuits to prevent fatigue and breakage?
- Are all your critical circuits fused or protected with circuit breakers close to the power source?
- Are you labeling your wires and connections for easier maintenance later?


### System Safety

- Are you using properly rated fuses or breakers for each part of the system (panels, controller, batteries, inverter)?
- Do you have a disconnect switch or method to shut down the system in case of emergency?
- Have you checked that all connections are tight, clean, and corrosion-resistant?
- Are you protecting battery terminals from accidental short circuits (covers, boots, etc.)?
- Do you have basic fire protection nearby (such as a fire extinguisher rated for electrical fires)?


### Other Important Considerations

- Have you estimated your daily energy usage and matched your panel size and battery bank to meet it?
- Are you planning for expansion if you think you'll add more panels or batteries later?
- Have you allowed space for ventilation around batteries, inverters, and charge controllers?
- Do you know how to monitor your system (basic meters, battery monitors, or smartphone apps)?
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTkyOTc1ODEwM119
-->