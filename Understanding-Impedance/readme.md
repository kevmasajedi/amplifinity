# Chapter 3: Understanding Impedance

To grasp the concept of impedance, let's break it down into two main types: resistive and reactive. 

**Resistive impedance** is the type we're most familiar with. It relates to Ohm's Law, the fundamental principle of electricity that most of us learned in school. On the other hand, **reactive impedance** involves inductors and capacitors, elements that 'react' to changes in voltage or current. Both are important in the realm of audio, but for our introduction, we'll focus on resistive impedance.

Now, let's consider a sound card that provides 1 volt RMS (Root Mean Square - the 'effective' or 'equivalent' DC voltage) but can only provide 1 milliampere (mA) of current. The impedance of this sound card would be 1 kilo-ohm, according to Ohm's Law (Voltage = Current x Resistance).

If you measure the output voltage of the sound card with a multimeter in True RMS AC mode, you'll see a reading of 1 volt. But what happens if we connect this sound card directly to a speaker with an impedance of 4 ohms?

To produce 1 volt across a 4-ohm speaker, the sound card would need to deliver 250 mA (according to Ohm's Law). However, our sound card can only provide 1 mA. So, when connected to the 4-ohm speaker, the sound card can only produce around 4 millivolts RMS. The voltage drops significantly because the sound card can't provide the current needed to maintain 1 volt across the lower impedance of the speaker.

This example underscores why understanding impedance is crucial when dealing with audio equipment. It helps us make informed choices, ensuring that our devices can interact effectively and deliver the best possible sound quality. And as we continue on our audio journey with Amplifinity, we'll delve deeper into these concepts.

## Introduction to Impedance

In the visual model below, consider the AC voltage source as the output of our sound card, complete with its equivalent impedance, represented by the resistor connected to it. Here, the amplifier is shown as a triangle, which is a common symbol for amplifiers in electronic schematics. Across the amplifier's terminals, we've placed another resistor, which represents the amplifier's equivalent impedance.

In this simple model, we're using resistors to represent the impedance of the sound card and amplifier. Remember, impedance isn't just resistance, but for our introduction, we're sticking to resistive impedance to keep things straightforward.

<p align="center"><img src="/Understanding-Impedance/pics/1.png?raw=true" width="720px" /></p>

In our simplified model, we assumed that the output impedance of our preamplifier (the sound card) is 50 ohms, which is a common approximation. However, keep in mind that the actual value might be different, and it's not safe to assume 50 ohms under all conditions.

Now, suppose the input impedance of our amplifier is also 50 ohms. If we feed a 1V RMS signal from the preamp into this setup, we'll end up with only 0.5V at the amplifier. 

Why is that? Well, this comes down to the principle of voltage division in circuits. When two resistors (or impedances) are in series, the total voltage gets split across them based on their relative values. Here, our preamp output and amplifier input have the same impedance, so the input voltage is divided equally between them, halving our voltage.

So, to prevent this waste of voltage, we should aim for a high input impedance for our power amplifier. The higher the amplifier's input impedance compared to the preamp's output impedance, the larger the fraction of the input voltage that gets across to the amplifier.

However, if we swing to the other extreme and choose an excessively high input impedance (say, 1 megaohm), we risk running into another issue: noise. The world is not a perfect place and neither are our cables, so our audio signal can pick up noise as it travels from the preamp to the power amplifier. This noise usually has a very low power level and so doesn't significantly affect a circuit with low impedance. But with a 1 megaohm input impedance, this noise can be amplified and start to interfere with our audio signal.

So, where does that leave us? In practice, a good compromise is to aim for an input impedance of around 5K to 10K ohms for a power amplifier. This value is high enough to keep most of the preamp's output voltage from being lost across the amplifier's input, while low enough to minimize noise pickup.

Thus, the process of choosing impedance values is a balancing act, one of many in the design of audio equipment.

<p align="center"><img src="/Understanding-Impedance/pics/2.png?raw=true" width="720px" /></p>
