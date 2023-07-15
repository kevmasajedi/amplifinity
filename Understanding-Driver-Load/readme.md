## Chapter 3: Understanding Driver Load

Let's talk about a parameter you may be familiar with when choosing a speaker driver - the impedance, which is often mistaken for resistance. If you've ever picked out a speaker driver, maybe for your car's sound system, you'll likely have seen these impedance values: 4, 6, 8, and less commonly, 2 ohms. Headphones typically have higher impedance values, but let's focus on loudspeakers for now.

So, let's say you've built your power amplifier and you want to test its tolerance for different loads. How do you do that? By using resistors of similar value to the speaker impedance! However, this may lead some to protest, "But speakers have reactive impedance too! Their impedance changes across the audio frequency spectrum due to the parasitic capacitance and inductance of the drivers." And they'd be right! But here's the thing...

Currently, there's no better way to test audio power amplifiers in the real world than using high-power resistors. While it's true that speakers' impedance can change with frequency due to inductive and capacitive elements, resistive loads provide a consistent, reliable benchmark to test your amplifier's performance.

And here's the comforting bottom line: if your amplifier can successfully drive a speaker with a low impedance (like 2 ohms) while maintaining low Total Harmonic Distortion (THD), then it's a safe bet that the THD will be even lower with higher impedance speakers. Essentially, driving low impedance speakers is more demanding because they require more current to generate the same voltage. Yes, that's our good old friend Ohm's law again! So, if your amplifier can handle the tougher test, it'll breeze through the easier ones.

Indeed, in a large range of frequency spectrum, the parasitic reactive elements actually result in an increase in the impedance of loudspeakers. This may seem like a complexity, but it often serves to lessen the load on your amplifier.

## Choosing Speaker Impedance

When it comes to choosing the impedance of your speakers, you have some freedom. You can freely use speakers with an impedance of 4 ohms or above. However, while 2 ohm subwoofers are common, using a 2 ohm driver for other spectrums is generally not recommended. The reason lies in the way Bipolar Junction Transistors (BJTs), used in the output stage of amplifiers, behave when they have to handle a large amount of current: they become more non-linear. Which results in a good amount of distortion.

Moreover, this increased current results in more voltage drop in cables and the amplifier's internal circuitry, leading to a decrease in efficiency. It also generates additional heat in the output transistors, necessitating larger heat sinks. Even then, the increased temperatures may reduce the lifespan of your power amplifier.

Fortunately, it's hard to find a 2 ohm driver for purposes other than subwoofers, and distortion at lower frequencies (the subwoofer range) isn't as crucial to our hearing. However, if you are concerned about efficiency, the size of the heat sink, and the lifespan of your amplifier, we recommend using drivers with an impedance of 3 ohms or higher even for subwoofers. 

Why is this? Because some 2 ohm loads can have even lower impedance at certain frequencies, approaching 1 ohm. This can trigger the amplifier's short-circuit protection and result in an unpleasant distortion known as clipping. Clipping sounds like the audio is being abruptly "cut off" or "clipped," hence the name. This sudden, harsh alteration in the signal can permanently damage tweeters, the small speakers responsible for reproducing high frequencies, due to their delicate construction and inability to handle such sudden, powerful shifts in the signal.

## Section: Power Delivery

When examining the specifications of commercial amplifiers, you might notice that their output power is listed separately for different speaker impedances. For instance, you may see specs like "200W into 8 ohms" and "400W into 4 ohms". As you've observed, these values usually double when the impedance is halved.

But why is this the case? Let's take a look at a practical example. Suppose an amplifier is trying to develop a 24V voltage across an 8 ohm driver. According to Ohm's law, this would require an output current of 3A. However, if the same voltage were developed across a 4 ohm driver, the required current would double to 6A. As we know, electrical power is calculated by multiplying the voltage by the current. Hence, the power output doubles.

However, this isn't always the case. Due to energy losses associated with higher currents demanded by lower impedance loads, the actual power delivered to a 4 ohm load may be less than double relative to an 8 ohm load. For example, an amplifier specified to deliver 200W into 8 ohms may only deliver around 320W into 4 ohms. 

These losses are mainly due to overheating and voltage drops within the amplifier's circuitry. But the exact amount of these losses can vary and depends on several factors including the design of your circuit, the quality of the cables, and the types of transistors used. Hence, it's essential to keep these factors in mind when deciding about your amplifier's specifications and to ensure your system is optimized for your specific requirements.