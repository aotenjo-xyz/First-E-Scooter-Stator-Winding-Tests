# Winder Max: First E-Scooter Stator Winding Tests
<img width="4096" height="3072" alt="Winder Max" src="https://github.com/user-attachments/assets/112f02e5-00fb-4b15-b753-492f3ad8c5c4" />

In my previous update, I upgraded my DIY winding machine to handle larger, heavier stators and proposed a gear-driven mechanism to support the stator during winding.

Now, I’ve assembled the next iteration of **Winder Max** and started winding tests with **0.3 mm enameled copper wire**.

There’s still plenty to improve, but I can finally test the mechanical changes under actual winding conditions.

## From Printed Parts to Machined Components

My earlier winding machines handled small drone motors, gimbal motors, and larger agricultural drone motors. Moving to thicker e-scooter stators means dealing with a larger payload while keeping the winding motion controlled and the wire insulation intact.

For this build, I replaced some of the less rigid 3D-printed components with custom machined parts. To get the precision I needed for this build, I sourced my custom components from JLCCNC, my go-to CNC fabrication service.

<img width="3690" height="2207" alt="M1 base v0 3" src="https://github.com/user-attachments/assets/241e702b-bf9a-4bfa-a86a-8bd1aeb57964" />

I’m keeping a combination of machined and printed parts: machined components where I need rigidity, and smaller printed components where I’m still experimenting with the geometry.

## Ordering the Custom Parts

I ordered the machined components through [JLCCNC](https://jlccnc.com/?from=yuchicnc).

The process starts with uploading the 3D models, selecting the material and finish, and specifying the quantity. Drawings and additional requirements can communicate critical dimensions and other details needed for the assembly.

After reviewing the quotation and manufacturing details, the next step is submitting the order.

For a project like this, it helps to think about which components are ready to manufacture and which are likely to change during testing. I’m trying to keep the frequently modified features in small, replaceable parts.

## Improvement 1: A Sheet-Metal Fin with Printed Adapters

<img width="2724" height="2525" alt="fin" src="https://github.com/user-attachments/assets/7d50ef38-e9bf-4972-ad07-8f0d8d209a79" />

One component that needed a rethink was the curved guide part I call the **fin**.

Previously, I printed the entire fin in PLA. This worked as a way to experiment with the shape, but as the stators became thicker, the fin also became larger. Every design adjustment meant reprinting the whole part.

The updated design combines:

- A sheet-metal fin.
- Small, replaceable 3D-printed adapters.
- Slotted mounting holes for adjustment.

Now, I can modify the adapters while reusing the metal fin. This reduces the amount of printing needed for each iteration.

The slots also make the design more flexible. The previous fin was specific to one stator size, while the new version can accommodate a range of similar stator sizes by adjusting its position and changing the adapters.

That should make it much easier to experiment without producing a completely new fin each time.

## Improvement 2: A Gear-Driven Stator Support

The other major change is the stator-holding mechanism.

In several YouTube videos of industrial winding machines for large BLDC motors, I noticed pneumatic actuators being used to hold the stator steady during winding. 

<img width="2654" height="1568" alt="industrial-winding-machine-example" src="https://github.com/user-attachments/assets/7051cac8-f45c-4477-953c-ceddcb570993" />

<img width="2578" height="1632" alt="pneumatic-actuator-push-stator" src="https://github.com/user-attachments/assets/524ac118-1ff1-4a1d-9004-9ce09123c3fa" />

For Winder Max, I wanted to avoid adding an air supply and a separate actuator, so I designed a gear-driven support that uses the machine’s existing motion.

As the stator moves forward, a **rack-and-pinion mechanism brings a support against it from behind**.

<img width="641" height="514" alt="rack-and-pinion mechanism" src="https://github.com/user-attachments/assets/126d41e8-4d36-4984-9fa2-2ff39649e71a" />

The goal is to support the stator automatically as it enters the winding position.

In my previous update, this was still an untested idea. Now, the mechanism is assembled, and I can observe how it behaves during winding.

It isn’t holding firmly enough yet. The stator still moves slightly, so I need to refine the geometry, fit, and way the support applies force.

The mechanism is still experimental, but these tests give me something concrete to improve.

## First Winding Runs with 0.3 mm Wire
<img width="4096" height="3072" alt="winding result" src="https://github.com/user-attachments/assets/764b6d2a-83f9-4b0c-afc2-5de15cd1e495" />

With the updated machine assembled, I started testing with **0.3 mm enameled copper wire**.

The failure rate is still high. Moving the stator through the winding sequence is only part of the challenge—the wire also needs to follow the intended path without snagging or damaging its insulation.

These runs are helping me evaluate the structural changes, wire guidance, and stator support together.

At this stage, I’m treating the machine as a development prototype. The next step is to identify the causes of failed runs, make targeted changes, and repeat the tests.

## What Comes Next?

My priorities are to:

- Reduce stator movement during winding.
- Refine the fin and wire-guiding geometry.
- Improve the consistency of repeated winding runs.

My goal is to make Winder Max reliable enough to release and help people automate this repetitive task.

Thanks to **JLCCNC** for supporting this iteration. If you need custom machined parts for your own project, you can check out their service here: [JLCCNC — Custom CNC Machining](https://jlccnc.com/?from=yuchicnc).

And if you’ve worked with winding machines or mechanical stator supports, I’d love to hear about your experience.

Thanks for reading!

For more about this project, go to the links below:

[Website](https://aotenjo.xyz) | [YouTube](https://www.youtube.com/@yuchi0.1) | [Instagram](https://www.instagram.com/aotenjo.xyz) | [TikTok](https://www.tiktok.com/@yuchi0.1)
