# Turbofan Engine Gas Generator with 239 kN Take Off Thrust

Bachelor thesis project
National Aerospace University Kharkiv Aviation Institute
Faculty of Aircraft Engines
Aircraft Engines Design Department

Author: Mudassir Saiyed Mohammad
Supervisor: Professor Sergiy Bezugly
Thesis code: XAI.203.240F.22S.134.EN
Year: 2022

## Project overview

This project is the preliminary design and analysis of a three shaft turbofan engine gas generator for a heavy cargo aircraft.

The work started from a D 18T class prototype engine. The aim was to calculate a modified engine cycle, match the compressor and turbine, design the compressor flow path, profile the compressor rotor blade, check strength and vibration behaviour, and plan manufacturing operations.

This was not a CFD project alone. It was a full engine design project, from thermodynamics to blade geometry, stress checks and manufacturing.

## Main result

The calculated engine produced higher specific thrust than the prototype baseline.

Prototype specific thrust:

312.38 N s/kg? No. That is the new design.

Correct comparison:

Prototype specific thrust = 300.654 N s/kg

New design specific thrust = 312.38 N s/kg

The gain is:

```text
Specific thrust gain = ((312.38 − 300.654) / 300.654) × 100
                     = 3.90 percent
```

The take off thrust also increased:

```text
Prototype thrust = 230 kN
New design thrust = 239 kN

Thrust gain = ((239 − 230) / 230) × 100
            = 3.91 percent
```

This does not mean the engine was wind tunnel tested. It means the new cycle and gas path calculation gave a better performance result than the prototype reference data used in the thesis.

## Main engine data

Take off thrust: 239 kN

Prototype take off thrust: 230 kN

Bypass ratio: 5.60

Compressor pressure ratio: 26.2

Turbine inlet temperature: 1615 K

Compressor mass flow rate: 115.916 kg/s

Specific thrust: 312.38 N s/kg

Specific fuel consumption: 0.037686 kg/(N h)

## What engineering problem was solved

The design problem was not simply to increase thrust.

A gas turbine engine must be balanced as a whole system. If the compressor pressure ratio is raised, the turbine must supply the work. If turbine inlet temperature is increased, cooling becomes more important. If the compressor blade is profiled aggressively, it may give the required pressure rise but lose stability or increase vibration risk.

So the project asked practical questions:

1. Can the engine produce 239 kN take off thrust?

2. Can the specific thrust be improved compared with the prototype?

3. Can the compressor and turbine be matched so the work balance is possible?

4. Can the compressor flow path keep pressure, temperature and velocity within reasonable limits?

5. Can the compressor rotor blade turn the flow without excessive loading?

6. Can the blade avoid dangerous bending resonance?

7. Can the part be manufactured with a clear machining route?

## Thermodynamic cycle calculation

The first step was the engine cycle calculation.

The aim was to calculate the pressure, temperature, thrust and fuel consumption through the engine.

The main quantities were:

Total pressure

Total temperature

Specific thrust

Specific fuel consumption

Mass flow rate

Compressor work

Turbine work

Pressure losses

Cooling effect

The main design inputs were:

```text
P = 239000 N
m = 5.60
πc = 26.2
Tt4 = 1615 K
P0 = 101325 Pa
T0 = 288.15 K
M0 = 0
```

The cycle result was:

```text
Specific thrust = 312.38 N s/kg
Specific fuel consumption = 0.037686 kg/(N h)
```

The prototype values were:

```text
Prototype specific thrust = 300.654 N s/kg
Prototype specific fuel consumption = 0.0377 kg/(N h)
```

The engineering decision was clear:

The new design gave higher specific thrust while keeping specific fuel consumption slightly below the prototype value.

## Why specific thrust matters

Specific thrust shows how much thrust is produced per unit mass flow.

A higher value means the engine is producing more useful momentum change from the same amount of air through the core calculation.

For this project:

```text
ΔPsp = 312.38 − 300.654
     = 11.726 N s/kg
```

```text
Percentage gain = 11.726 / 300.654 × 100
                = 3.90 percent
```

This is the strongest performance result in the project.

It should be described as a calculated cycle and gas path improvement compared with a prototype baseline, not as a wind tunnel result.

## Pressure losses and cooling

Real engines lose total pressure through the inlet, ducts, combustion chamber and nozzles.

These losses were included using pressure recovery factors.

For the combustion chamber:

```text
σhydraulic = 0.970
σthermal = 0.980

σcombustion chamber = 0.970 × 0.980
                    = 0.951
```

This matters because total pressure loss reduces the pressure available for turbine expansion and thrust generation.

The turbine inlet temperature was 1615 K, so blade cooling had to be considered. Cooling protects the turbine but reduces efficiency because cooling air is taken from the compressor and mixed into the turbine flow.

The cooled turbine efficiency was estimated from:

```text
ηt = ηt uncooled − 0.000125 × (Tt4 − 1250)
```

This gave:

```text
ηt = 0.874
```

The engineering judgement here is that increasing turbine inlet temperature helps thrust, but it is not free. It adds cooling demand and turbine loss.

## Compressor and turbine matching

After the cycle calculation, the compressor and turbine had to be matched.

This is one of the most important parts of engine design because the turbine must provide the power required by the compressor and fan.

The matching calculation defined:

Spool work split

Number of stages

Rotational speeds

Flow path shape

Stage loading

Turbine work

Blade height limits

Hub and tip diameter limits

The final layout was:

```text
Fan: 1 stage
Low pressure compressor: 7 stages
High pressure compressor: 7 stages
High pressure turbine: 1 stage
Low pressure turbine: 1 stage
Fan turbine: 4 stages
```

The full compressor had 14 axial stages.

The design used a three shaft layout so each rotor group could operate closer to its own best rotational speed. This is important for compressor stability and efficiency.

## Compressor gas path calculation

The compressor gas path calculation checked how the flow changed stage by stage.

The compressor calculation gave:

Axial velocity distribution

Total pressure distribution

Static pressure distribution

Total temperature distribution

Static temperature distribution

Stage work

Stage pressure ratio

Stage efficiency

Reactivity coefficient

The compressor input data included:

```text
Mass flow rate = 115.916 kg/s
Compressor inlet total temperature = 324.6 K
Compressor inlet total pressure = 146000 Pa
Compressor pressure ratio = 18.093
LPC first stage tip speed = 335 m/s
HPC first stage tip speed = 415 m/s
Compressor exit axial velocity = 125 m/s
Total compressor stages = 14
```

The key engineering point is this:

A compressor is not judged only by pressure ratio. It must raise pressure while keeping velocity, flow angle, stage loading and stability under control.

The calculated pressure and temperature distributions followed the normal pattern expected from an axial multistage compressor.

## Compressor blade profiling

The first stage high pressure compressor rotor blade was profiled using blade element calculations.

The blade was calculated at five spanwise sections:

Tip

Upper span

Midspan

Lower span

Hub

The profiling used:

Velocity triangles

Axial velocity

Tangential velocity

Relative velocity

Inlet and outlet flow angles

Flow turning angle

Cascade solidity

Blade chord

Blade pitch

Blade count

The main flow turning calculation was:

```text
β1 = 35.051 degrees
β2 = 53.925 degrees

Δβ = β2 − β1
   = 53.925 − 35.051
   = 18.874 degrees
```

The cascade design reference gave:

```text
Δβ at b/t = 1 = 18.43 degrees
```

The loading parameter was:

```text
E = 18.874 / 18.43
  = 1.024
```

This gave a selected solidity:

```text
b/t = 1.03
```

This is an important aerodynamic decision.

If solidity is too low, the blade row cannot turn the flow enough.

If solidity is too high, friction, blockage and loss increase.

The blade count came from the selected chord and pitch.

Blade height:

```text
h = (Dtip − Dhub) / 2
  = (0.8447 − 0.6840) / 2
  = 0.08035 m
```

Midspan chord using aspect ratio 3:

```text
bmid = 0.08035 / 3
     = 0.02678 m
```

Pitch:

```text
tmid = bmid / (b/t)
     = 0.02678 / 1.03
     = 0.026007 m
```

Blade count:

```text
Z = π Dmid / tmid
  = π × 0.7685 / 0.026007
  = 92.83
```

Final selected blade count:

```text
Z = 93 rotor blades
```

This is the part I care about most as an engineer. The blade count was not guessed. It came from the flow turning requirement, solidity, chord and pitch.

## Strength check

The compressor blade, blade lock and disc were checked for strength.

The blade is a critical part because it carries centrifugal load and aerodynamic load at high rotational speed.

The project used the take off operating condition as the design case because this is where speed and loading are high.

The aim was to check whether the blade and its fixing could carry the required load with enough margin.

This links the aerodynamic design to structural safety. A blade profile is not useful if the root, disc or blade body cannot survive the operating load.

## Frequency analysis

The blade was also checked for bending vibration.

This matters because compressor blades pass through non uniform flow caused by guide vanes, stators and struts. These create periodic forcing on the rotor blade.

If the forcing frequency matches the blade natural frequency, resonance can occur. The blade vibration amplitude can then grow and damage the blade.

The analysis treated the blade as a cantilever fixed at the disc.

The first bending mode was considered the most important because it is usually the most dangerous for early resonance checks.

The main idea was:

```text
Avoid resonance when:

forcing frequency ≠ blade natural frequency
```

The natural frequency found for the compressor blade was:

```text
f = 338.65 Hz
```

The engineering decision was to compare this natural frequency with the possible excitation harmonics from the engine. The aim was to check whether the blade would be excited dangerously in normal operation.

Future work should include a clearer Campbell diagram, finite element mode shapes, stress response at resonance, damping assumptions and comparison with test data.

## What was checked against evidence

The BEng project used prototype engine data as the reference for performance comparison.

The gain in specific thrust was calculated against the D 18T prototype baseline.

This is not the same as wind tunnel validation.

A wind tunnel or compressor cascade test would be the next step to check the blade aerodynamics directly.

The honest statement is:

The project shows calculation based optimisation against a prototype reference.

It does not claim wind tunnel validation.

Future testing could use:

Compressor cascade wind tunnel test

Pressure taps across blade surfaces

Five hole probe wake measurement

Flow angle measurement downstream of the cascade

Loss coefficient measurement

Comparison with CFD for the same blade section

This would turn the blade design from calculation based evidence into test correlated evidence.

## Link to my later CFD work

My later CFD validation work follows the same engineering thinking.

In the turbulent jet CFD project, I compared CFD against experimental data and used the data to choose the turbulence model. The decision was not made from one contour plot. It was based on whether the model reproduced centreline velocity decay, shear layer growth, velocity field and temperature field.

That is the same judgement I would apply as future work on this engine project:

Check the calculation first

Run CFD with a controlled mesh

Compare with test data

Look at the physics

Then decide whether the design is reliable

## How I would develop this project next

The project can be improved in several honest and useful ways.

### 1. Compressor blade CFD

Run CFD on the first stage HPC blade section.

Check:

Surface pressure

Mach number

Separation risk

Wake loss

Exit flow angle

Loss coefficient

Incidence sensitivity

### 2. Cascade wind tunnel correlation

Build or test a 2D blade cascade section.

Measure:

Inlet flow angle

Outlet flow angle

Static pressure

Wake profile

Total pressure loss

Then compare the measured values with CFD and the original blade element calculations.

### 3. Full compressor stage CFD

Model the rotor and stator together.

Check:

Rotor exit flow

Stator inlet angle

Pressure rise

Stage efficiency

Tip leakage if clearance is included

Secondary flow near hub and tip

### 4. Better vibration work

Create a finite element model of the blade.

Check:

First bending mode

Second bending mode

Torsional mode

Mode shapes

Stress distribution

Campbell diagram

Margin from engine order excitations

### 5. Better cycle comparison

Repeat the cycle calculation with sensitivity studies.

Vary:

Compressor pressure ratio

Turbine inlet temperature

Bypass ratio

Cooling air fraction

Combustion chamber pressure loss

Nozzle loss

Then check how each change affects specific thrust and fuel consumption.

## Repository contents

01 Thesis Document

Mudassir Saiyed 240F.pdf

Complete bachelor thesis with calculations, figures and design method.

02 Technical Drawings

BP Engine.PDF

Engine arrangement and parameter distribution.

Gas generator 2.PDF

Detailed gas generator drawing.

SolidWorks

Gas generator assembly.

Compressor blade model.

Engineering drawings.

03 Presentations

Defense Presentation.pptx

Final project defence presentation.

04 Results Figures

Exported images from CAD models.

Flow path diagrams.

Blade profile figures.

Parameter plots.

## What this project shows

This project shows that I can work through an engineering problem from first principles.

I calculated the cycle.

I matched the compressor and turbine.

I designed the compressor flow path.

I profiled a compressor blade from flow angles and solidity.

I checked strength.

I checked bending vibration.

I considered manufacturing.

The strongest part of the work is the connection between physics and decisions. The design was not judged by one number. It was judged by thrust, fuel consumption, pressure ratio, temperature, stage loading, blade geometry, strength and vibration risk together.

## Academic note

This was completed as a bachelor thesis at the National Aerospace University Kharkiv Aviation Institute in the Aircraft Engines Design Department.

It is shared as an engineering portfolio project and academic reference.

## Contact

Saiyed Mudassir

LinkedIn: https://www.linkedin.com/in/saiyedmudassir18/

GitHub: https://github.com/MudassirCFD
