# Solar Workshop Outline

## Introduction

- Who we are and our experience
- Brief description of workshop
- Discourage from taking notes, there is a zine online, and handout.
- Please feel free to interupt and ask questions, but we do want to make it through everything and we'll be around all weekend if you have more in-depth questions or questions specific to your situation
- Go over agenda
- What it's not going to be
    - Disclaimer that there's a lot that goes into building a solar power system, some of the choices about things we've already made for you. So if you're starting from scratch make sure you know what to consider.
- Guage people's level of experience somehow?

## Basic solar systems and what were building

- Put up diagram of solar components
- One sentance description of each
- What were building

## Put electrical concepts on board

This is what we're going to talk about in the next sections

- Saftey
- AC vs. DC
- Circuits
- Polarity
- Voltage
- Current / Amperage
- Power / Wattage

## Electrical saftey

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

## AC vs. DC

(Show or draw diagram of different wave forms)

Electricity can flow in two different ways: Alternating Current (AC) and Direct Current (DC). Both are used in electrical systems but have different characteristics and applications.

You do not need to really know any of this for the rest of our purposes; besides that we will be using mostly DC unless otherwise specificed, and that AC and DC power are not interchangable or mixable.

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

## Why what were doing is 12v DC

- All solar panels produce direct current, so with solar were in DC world unless we use what's called an inverter to produce alternating current
- 12V DC is standard for smaller solar setups:
	- The components are more readily available.
	- It's all you need for most portable applications.
	- Because all vehicles produce 12v it's interoperable with vehicle systems
- A number of radios that don't have their own batteries operate at 12v, and since getting clean 12v power is often a concern when operating sensative radio equipment, this will provide it without the need for a dedicated power supply.

## Circuits

A circuit is simply a pathway that allows electricity to flow from a power source (like a battery or solar panel), through wires and devices (such as lights, appliances, or other loads), and back to the power source.

For electricity to move and do useful work, the circuit must be complete — meaning there is a continuous path with no breaks. If the circuit is broken (like when a switch is turned off or a wire is disconnected), the flow of electricity stops.

At its core, a circuit includes three basic parts:

- Power Source: Provides the energy (e.g., a battery, solar panel, or generator).

- Conductors: Wires that carry the electrical current.

- Load: Any device that uses the electricity. You all have a load at your station that you've choosen. 

(Have then shout out their loads or other examples of loads)

## Intro to batteries and polarity

### What is a battery

A battery uses chemical reactions to store energy for use when the sun isn’t shining. The two most popular options are:

- **Lead-Acid (AGM, Gel):** Affordable but lower lifespan.
- **Lithium-Ion (LiFePO₄):** More efficient, longer-lasting, but higher cost.

### What is polarity

**Polarity** refers to the positive (**+**) and negative (**\-**) orientation of a DC circuit.

Red is usually positive and black is usually negative.

- **Correct polarity** ensures that devices receive power properly.
- **Reversed polarity** can damage sensitive electronics, prevent charging, or cause a short circuit.
- In solar power systems, **battery terminals, solar panels, and charge controllers must be connected with correct polarity** for efficient operation and safety.

A multimeter should be used to confirm **polarity** before making connections.

### What is a multimeter

A multimeter is one of your most important electronics tools. 

It is used to measure various electrical quantities like voltage, current, and resistance.

### Finding polarity w/ a multimeter

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

## Connecting load to battery

Now we're going to connect your load to the battery temporary, to test it and to create a complete circuit.

There are fuses on the wires you have, ignore them for now and we'll come back to that (or do we have them solder in the fuse holders?)

HOWEVER: you should never mess around with things like this without fuses, remember that.

### How to use wire strippers

- Wire strippers are another very important tool.
- Explain determining which hole to use.

### How to use a box cutter to strip wire?

### Making the connection

- Just twist the wires or use wire nuts to connect
- See if the load is getting power

## Fluid dynamics metaphor intro

Let’s try to explain some key electrical concepts using the analogy of water flowing through a pipe.

When water flows through a pipe, increasing or decreasing either the size of the pipe or the flow rate of the water will accordingly increase or decrease the ammount of water you get out of the end of the pipe. Let’s look at three electrical concepts and how they relate to the water in the pipe:

**Voltage** (V_)_ - (measured in **volts**, represented as V) is the electrical potential, or size of the pipe. It’s not exactly correct, but it helps to think of it as a bigger pipe means there’s a bigger potential amount of water that could flow through, and a higher voltage the larger potential for electricity you have.

Voltage can also be helpful to think about in terms of compatability of different components in a circuit. A circuit with components rated for different voltages will not work and may cause damage or fires. Components even of the same voltage that are meant for AC or DC power (which will be covered later) also cannot be mixed. For example, pretty much everything in a vehicle is 12 volts DC, while most everything in your house is 120 volts AC. 

**Current** (I) - (measured in **amps**, represented as A) is the rate at which electrons flow through a circuit, or in the pipe how fast water is moving through it. The faster then water flows, the more water you have at the end. The higher the current (or amperage or amps) the more eletricity you have.

**Power** (P) - (measured in **watts**, represented as W) is the ammount of electricity used or produced. So in the pipe it’s the ammount or volume of water you get out at the end of the pipe.

_Bonus that you probably won’t use for our purposes but you might as well know:_

**Resistance** (R) - (measured in **ohms**, represented as Ω) The opposition to the flow of electric current. So in our water example it’s any kink or obstruction in the pipe.

## Voltage and solar panels

### What is a solar panel?

Solar panels, some times refered to as PV or photovoltaic panel or module, convert sunlight into a flow of electrons (or an electrical current) using the photovoltaic effect.

- Made of a number of solar cells wired together.
- Typically silicon-based.
- Rated by wattage (W), indicating power output in ideal sunlight.
- Also have a voltage rating, they typically say higher than the system size (i.e. 12v panels will be like 15-16v and put out that much).
- The voltage doesn't matter if you're using a MPPT charge controller which well come back to, but does matter for the charge controllers were using.

Types: Monocrystalline, Polycrystalline, Thin-Film (varying efficiency & cost).

### Reading the solar panel label

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

### Use multimeter to determine PV voltage

- Remember: voltage is the electrical potential, or size of the pipe.
- What we're going to measure is Open Circuit Voltage (Voc), which is not neccessarily the same as Voltage at Max Power (Vmp) which is when it is connected to a charge controller or load.
- Probe panels and batteries w/ multi meter and writing down voltage, in full sun
- Use same multimeter settings at before
- Play around with what happens when you shade them

### Solar panel positioning

#### 1\. Solar Panel Positioning

**Direction (Azimuth Angle):**

- **In the Northern Hemisphere** → Face panels **South**
- **In the Southern Hemisphere** → Face panels **North**
- **If adjustable**, panels can be slightly turned **Southeast or Southwest** to optimize for morning or afternoon sun, depending on energy usage patterns.

#### 2\. Solar Panel Angle (Tilt) for Maximum Output

<media-tag src="https://files.cryptpad.fr/blob/ce/ceed8061c36ea161ee4cb98a7ab73f3d347a1be3acdf5a0b" data-crypto-key="cryptpad:F3U4/nM9XyAoYxeHww2sDsh4hxn8m/c5yFu7MgRo8hY="></media-tag>

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

## Measuring current 

Remember: current is (measured in **amps**, represented as A) is the rate at which electrons flow through a circuit, or in the pipe how fast water is moving through it. The faster then water flows, the more water you have at the end. The higher the current (or amperage or amps) the more eletricity you have.

### Finding short circuit current of PV panel

1. Set your **multimeter to DC amps (A or mA mode)**.
2. Place the panel in **full sunlight**.
3. Connect the **positive probe to the positive panel wire**.
4. Connect the **negative probe to the negative panel wire**.
5. Compare the reading to the **Isc value on the label**.

Write down the value when youre done.

**Warning:** Some multimeters can only handle small currents (e.g., 10A max). If the panel exceeds this, use a **clamp meter** or a proper charge controller test instead.

**Good result:** Output **at least 70-80% of rated power** under good sunlight.  
**Bad result:** If power is much lower than expected, the panel has **cell degradation, dirt, or internal failure**.

### Finding the current of your load

Set your multimeter to DC amps (A or mA mode). Larger than expected for load (which is ?)

Place one probe on the battery wire and the other on the load wire for positive.

(Just demostrate and explain this)

This is how much power it is comsuming, so it may change as you use the device and it uses more power (if it's something that can change, have them mess around).

Write down what the highest amprage reading you got on your paper.

### Parallel vs. Series

Wiring **solar panels** and **batteries** in series or parallel affects the **voltage and current** of the system. Understanding the differences helps in designing an efficient **12V solar power system**.

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

## Power formula

Let's talk about power again:

**Power** (P) - (measured in **watts**, represented as W) is the ammount of electricity used or produced. So in the pipe it’s the ammount or volume of water you get out at the end of the pipe.


There is one important relationship amung these concepts that will help you immensly in working on solar power projects (and probably your every day life if you ever look at electrical appliance labels). But that means we have to introduce a formula - the formula for power. Remember power is just the amount of water you get at the end of the pipe once you’ve adjusted the size of the pipe and the flow rate of the water.

```math
  Power(P) = Voltage(V) \times Current(I)
```

It might also be useful to think of it or remember it by the units of measure like:

```math
  Watts (W) = Volts (V) \times Amps (A)
```

All you do to get power (watts) is multiple voltage (volts) by current (amps). Wattage tells you how much electricity something will use without knowing the volts or amps.

The power formula also allows you to find voltage if you have current and power (_V = P/I_) or current if you have voltage and power (I = P/V).

TODO: example of power formula

## Watt and amp hours of batteries and devices

When designing a solar power system, it’s essential to understand **Amp-Hours** (Ah) and **Watt-Hours** (Wh) to measure battery capacity and energy consumption.

### Amp-Hours (Ah)

An **Amp-Hour** (Ah) is a unit that measures **electrical charge capacity** over time. It tells you how much current a battery can supply for **one hour** before it is depleted.

```math
  AmpHours(Ah) = Current (A) \times Time (hours)
```

**Example:**

- A **100Ah battery** can provide:
- **100A for 1 hour**, or
- **10A for 10 hours**, or
- **1A for 100 hours**

However, this depends on battery efficiency and discharge rate.

### Watt-Hours (Wh)s

A **Watt-Hour (Wh)** is a measure of **energy**. It tells you **how much power a system can deliver over time**. Since power is measured in watts (W), Watt-Hours indicate the total energy available.

#### **Formula:**

```math
WattHours (Wh) = Volts (V) \times AmpHours (Ah)
```

#### **Example:**

- A **12V 100Ah battery** has: 

```math
    12V \times 100Ah = 1,200Wh

```
This means the battery can **deliver 1,200 watts for 1 hour** or **100 watts for 12 hours** (under ideal conditions).

#### Why Are These Important in Solar Power Systems?

- **Choosing the Right Battery Size:** Batteries are rated in **Ah**, but energy needs are often in **Wh**.
- **Estimating Energy Consumption:** Devices use **Wh** (e.g., a 50W fan for 5 hours = 250Wh).
- **System Efficiency:** Inverters and other components affect how much of the stored **Wh** can actually be used.

## Planning Your System Capacity

This is an example of how you would plan and figure out the components needed for a system that can run two ham radios and a light.

### Step 1: Determine Total Power Needs

1. List all radios and accessories.
2. Find each device’s **power rating (W)** and **operating hours per day**.
3. Use the formula:

```math
Total Energy (Wh) = ∑(Power(W) × Hours Per Day)
```

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
**For **300Wh/day** and **5 sunlight hours**:

300Wh / 5h = 60W

**Use a 100W solar panel** for extra capacity and cloudy days.

### Step 3: Select a Battery

- Convert **Wh to Ah** for a **12V battery**:

Battery Capacity(Ah) = Daily Energy (Wh) / Battery Voltage (V)

**Example:**

300Wh / 12V = 25Ah

**Use a 50Ah deep-cycle battery** to ensure reliable backup power.

### Step 4: Pick a Charge Controller

- Prevents overcharging and regulates power.
- Use the formula:

Charge Controller (A) = Solar Panel (W) / Battery Voltage (V)

**Example:**

100W / 12V = 8.3A

**Use a 10A or 15A charge controller** for safety.

- Have them calculate how long the device they have could be used with the other things they have

## Solar charge controllers

We're almost ready to connect everything but we've left out solar charge controllers.

The charge controller regulates the power from solar panels to prevent overcharging the battery. Can also help prevent battery from being over discharged.

(Talk about what they do and show them and where things go.)

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


## How things go together

(Revisit diagram of how things are connected, but we need wire and fuses in between)


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

### Wire Size and Voltage Drop

Proper wire sizing is **critical** in a solar power system to **prevent overheating, reduce power loss, and maintain efficiency**. One of the biggest factors in choosing wire size is **voltage drop**, which occurs when electricity travels through the wire and loses energy due to resistance.

Voltage drop happens depending on the length of the wire, its thickness, and the voltage and current running through it. Wires that are too thin or run too long introduce more and more resistence, which causes the voltage to drop. This can impact performance or you system, but also can start fires as the electricity lost is displaced as heat.

Wire sizes are measured in AWG (American Wire Guage). The lower the guage number the thicker the wire and the higher the guage number the thinner.

In order to properly size your wires you will need to know the maximum possible current (amps) running through them.

- For solar panels just add up the amprage of each panel (or use the power formula to convert watts to amps).

#### Determining Appropriate Wire Size

To detemine what size wire to use it’s best to use an online or phone based voltage drop calculator where you plug in the voltage, current (amps), and size of the wire run, and it gives you back the thickness you need to keep the voltage drop within the 3% maximum recommended drop range. You can also consult this table:

## Demo of melting wire

## Determine wire size needed for this project

Look at chart and values you wrote down.
- For panels to charge controller
- Battery to charge controller
- For charge controller to load.

### Fuses

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

```math
  {1000W \over 12V} = 83A
 
```

```math
  {83A \times 1.25} = 104A
```

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

## Demo of fuse blowing
## Calculating fuse sizes

- Between battery and charge controller
- Between charge controller and device

## Connecting the battery to the charge controller

- Crimping if we haven't already done that
- Always connect battery first, explain why

## Connecting panels to charge controller

- RC4 connector crimping

## Connecting device to charge controller

- Difference between connecting to charge controller and to battery

## Programming charge controller

## Inverters

## 12v fuse boxes

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


## Alternative Ways to Charge Batteries

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

### Charging from a Vehicle Alternator

A vehicle’s **alternator** generates DC power while the engine runs, which can be used to charge **house batteries in an RV, camper, or off-grid setup**.

#### Using a Battery Isolator (Basic Setup):

- Allows alternator to charge a second battery while **keeping it separate from the vehicle’s starter battery**.
- Uses a **Voltage-Sensing Relay (VSR)** to connect batteries only when the engine is running.
- When the vehicle is off, the relay **disconnects** to prevent draining the starter battery.

#### Using a DC-DC Charger (Better for Lithium & Deep-Cycle Batteries)

- A **DC-DC charger (20A-50A models)** ensures the house battery gets the correct charging voltage.
- Essential for **Lithium (LiFePO4) batteries**, since alternators don’t always reach their needed voltage.
- Provides **multi-stage charging** (Bulk, Absorption, Float).
- Protects the alternator from excessive load.


# Other Topics
## Batteries in depth

### Understanding Battery Measurements

Batteries are the heart of a small solar power system. Knowing how to read and understand their ratings is critical for designing, using, and maintaining your system properly. Here are the key measurements and what they mean:

#### Voltage

- **Nominal Voltage**: The standard working voltage of the battery (common values: 12V; 24V; 48V).
- **Actual Voltage**: Varies depending on the battery’s charge state; a 12V battery might range from 11.8V (nearly empty) to 14.4V (charging).

**Why It Matters**: Your inverter and charge controller must match your battery bank’s voltage.

#### Battery Capacity (Ah and kWh)

- **Amp-Hours (Ah)**: Measures how many amps a battery can deliver for how many hours.
  - Example: A **100Ah** battery can theoretically deliver **10A** for **10 hours**.
- **Kilowatt-Hours (kWh)**: Total energy stored, combining voltage and amp-hours.
  - Formula: **kWh = (Ah × V) ÷ 1000**
  - Example: A 12V, 100Ah battery = 1.2kWh of storage.

#### Depth of Discharge (DoD)

- **Definition**: How much energy you can safely take out of a battery before it should be recharged.
- **Expressed As**: A percentage (%).
- **Example**: If a battery has a **100Ah** capacity and you discharge it by **50Ah**, the DoD is **50%**.
- **Why It Matters**: Most batteries last longer if they are not fully discharged.  
  - Lead-acid batteries typically have a recommended DoD of **50%**.
  - Lithium batteries often allow a DoD of **80–90%** without harming lifespan.

#### State of Charge (SoC)

- **Definition**: How full the battery is at a given time, usually expressed as a percentage.
- **Example**: 100% SoC means fully charged; 0% means completely empty.
- **Why It Matters**: Monitoring SoC helps you avoid damaging deep discharges or overcharging your battery.

#### C-Rate (Charge/Discharge Rate)

- **Definition**: The rate at which a battery is charged or discharged relative to its total capacity.
- **Expressed As**: A number (like 1C, 0.5C, 2C).
- **Example**:
  - **1C** means charging or discharging the entire battery capacity in 1 hour.
  - **0.5C** means charging or discharging the full capacity in 2 hours.
- **Why It Matters**: Exceeding recommended C-rates can shorten battery life, cause overheating, or even damage the battery.

#### Cycle Life

- **Definition**: How many complete charge/discharge cycles a battery can handle before its capacity drops significantly.
- **Expressed As**: A number of cycles (e.g., 500 cycles; 2,000 cycles; 5,000 cycles).
- **Why It Matters**: Higher cycle life = longer battery lifespan; lithium batteries generally have a much longer cycle life than lead-acid batteries.


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

## Installation Longevity Considerations

A well-organized **solar power system** is not only more **efficient and easier to maintain**, but it also ensures **safety and durability** in various environmental conditions. Below are best practices for **cable management, weather protection, and battery storage.**

### Keeping a Solar Installation Neat

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

<media-tag src="https://files.cryptpad.fr/blob/b2/b275f06d2ea4ca292f9927dd2cdbb3bc455a1c87664eaebc" data-crypto-key="cryptpad:Eu1oRpnmnS2WtN4rkNuC+4ojNcc+C1QW60ATg9pou5c="></media-tag>

#### Battery Bank

- **Keep batteries out of direct sunlight** and extreme heat to extend lifespan.
- **For flooded lead-acid batteries**, install in a ventilated space to release hydrogen gas safely.
- **Seal cable entry points** in battery enclosures to prevent dust and pests.

#### Consider a Battery Box

Proper battery storage is helpful for safety, ventilation, and temperature control.


## Larger than 12V Systems

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

## Questions?