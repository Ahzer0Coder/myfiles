---
publish: true
created: 2026-05-12T21:16:22.797+03:00
modified: 2026-05-13T21:15:16.277+03:00
---

## 1. Determination of High Resistance by Leakage Method

- **Aim:** Study the behavior of a capacitor in an RC series circuit by analyzing charging/discharging processes, understanding the time constant (RC), and determining the resistance value.

- **Tools:** DC power supply, Capacitors, Resistors, Ammeter, Stopwatch.

- **Theory:**    A capacitor stores electrical energy.
  The charge stored during charging is given by $Q=Q_{0}(1-e^{-\frac{t}{\tau}})$.
  During discharge, the current decreases according to $I=I_{0}e^{-t/RC}$.
  Taking the natural logarithm gives $\ln I=\ln I_{0}-\frac{t}{RC}$, where $\tau = RC$ is the time constant.

- **Method:**
  1.Construct the circuit.
  2\. Close the switch to fully charge the capacitor.
  3\. pen the switch and record the variation of current $I$ with time $t$.
  4\. Plot a graph of $\ln I$ versus $t$.
  5\. Calculate the resistance using the slope relation: $\text{slope} = -\frac{1}{RC}$.

## 1. تعيين المقاومة العالية بطريقة التسرب

- **الهدف:** دراسة سلوك المكثف في دائرة توالي من نوع (RC) من خلال تحليل عمليتي الشحن والتفريغ، وفهم مفهوم ثابت الزمن (RC)، وتعيين قيمة المقاومة.

- **الأدوات:** مصدر جهد مستمر (DC)، مكثفات، مقاومات، أميتر، ساعة توقيت.

- **النظرية:** يقوم المكثف بتخزين الطاقة الكهربائية.
  تُعطى الشحنة المخزنة أثناء عملية الشحن بالعلاقة: $Q=Q_{0}(1-e^{-\frac{t}{\tau}})$.
  أما أثناء عملية التفريغ، فينخفض ​​التيار وفقاً للعلاقة: $I=I_{0}e^{-t/RC}$.
  وبأخذ اللوغاريتم الطبيعي للطرفين، نحصل على العلاقة: $\ln I=\ln I_{0}-\frac{t}{RC}$؛ حيث يمثل $\tau = RC$ ثابت الزمن.

- **طريقة العمل:**

1. قم بتوصيل الدائرة الكهربائية.
2. أغلق المفتاح لشحن المكثف بالكامل.
3. افتح المفتاح، وسجّل تغير قيمة التيار $I$ بدلالة الزمن $t$.
4. ارسم رسماً بيانياً يوضح العلاقة بين $\ln I$ والزمن $t$.
5. احسب قيمة المقاومة باستخدام علاقة الميل: $\text{slope} = -\frac{1}{RC}$.

## التجربة الأولى: تفريغ المكثف (High Resistance by Leakage)

**الهدف:** رسم العلاقة بين الزمن $t$ و $\ln(I)$ لإيجاد ثابت الزمن $RC$.

| Time $t$ (sec) | Current $I$ ($\mu A$) | $Ln(I)$ |
| :------------: | :-------------------: | :-----: |
|       10       |          1.2          |  -6.73  |
|       20       |          .6           |  -7.42  |
|       30       |          .3           |  -8.11  |
|       40       |          .2           |  -8.5   |
|       50       |          .1           |  -9.2   |

Slope =$\frac{-8.5+7}{50-20}=-0.05$
RC = $\frac{-1}{slope}=\frac{-1}{-0.05}= 20\Omega$

```
    ┌──────────┐
    │          │
    │  مقاومة  │ R (عالية)
    │          │
    ├────┤     │
    │    │     │
    │   ┌┴┐    │
    │   │C│    │
    │   └┬┘    │
    │    │     │
    └────┼─────┘
         │
       فولت متر (V)
```

```chart
type: line
labels: [10, 20, 30, 40, 50]
series:
  - title: Ln I (mA)
    data: [-6.73, -7.42, -8.11, -8.5, -9.2]
tension: 0
beginAtZero: false
width: 100%

```

---

## 2. Characteristic Curve of Diode

- **Aim:** Study and draw the characteristic curve of a metal rectifier diode, and calculate its internal resistance ($R_{in}$).

- **Tools:** DC power supply, Diode, Resistor, Ammeter, Breadboard.

- **Theory:** A PN junction diode allows electric current to pass in one direction. Forward bias decreases the depletion region (acts as a conductor). Reverse bias increases the depletion region (acts as an insulator).

- **Method:**

  1. Connect the circuit in forward bias using a milliammeter.

  2. Record current ($I$) for different voltages ($V$) and draw the relation.

  3. Connect the circuit in reverse bias using a microammeter and plot on the negative axes.

  4. Find $R_{in}$ from the slope of the straight part of the curve.

## التجربة الثانية: خصائص الدايود (Diode Characteristics)

**الهدف:** رسم منحنى الجهد والتيار في حالتي الانحياز الأمامي والعكسي للدايود العادي.

**1. الانحياز الأمامي (Forward Bias):**

| Voltage $V$ (Volts) | Current $I$ (mA) |
| :---: | :---: |
| 0.0 | 0.0 |
| 0.4 | 0.0 |
| 0.6 | 1.0 |
| 0.7 | 5.0 |
| 0.75 | 15.0 |
| 0.8 | 30.0 |

**2. الانحياز العكسي (Reverse Bias):**

| Voltage $V$ (Volts) | Current $I$ ($\mu A$) |
| :---: | :---: |
| 0.0 | 0.0 |
| -2.0 | 0.0 |
| -4.0 | 0.0 |
| -6.0 | 0.0 |

---

## 3. Zener Diode Characteristics

- **Aim:** Study the effects of forward and reverse bias on the Zener diode current and determine Zener breakdown voltage.

- **Tools:** DC power supply, Zener Diode, Resistor, Ammeter, Breadboard.

- **Theory:** Zener diodes are designed to operate in the reverse breakdown region. After reaching the breakdown voltage, the current increases widely for a very small change in voltage.

- **Method:**

  1. Connect the diode in forward bias with a series limiting resistor.

  2. Slowly increase voltage, measure current ($I$) and voltage across the diode ($V_D$).

  3. Plot $V_D$ vs $I_D$ and calculate forward resistance from the slope.

  4. Repeat in reverse bias to calculate the breakdown voltage.

## التجربة الثالثة: خصائص زينر دايود (Zener Diode)

**الهدف:** إيجاد جهد الكسر (Breakdown Voltage $V_z$) للزينر في حالة الانحياز العكسي. (بافتراض $V_z = 5.1V$)

**الانحياز العكسي (Reverse Bias - Zener Region):**

| Voltage $V$ (Volts) | Current $I$ (mA) |
| :---: | :---: |
| 0.0 | 0.0 |
| 2.0 | 0.0 |
| 4.0 | 0.0 |
| 5.0 | 1.0 |
| 5.1 | 15.0 |
| 5.2 | 30.0 |

---

## 4. Determination of a Condenser Capacitor by Vectors Method

- **Aim:** Determination of a condenser capacitor by vectors method.

- **Tools:** AC power supply, Voltmeter, Capacitor, Resistor, Breadboard.

- **Theory:** In a series RC circuit, current is the same across elements. For a resistor, voltage and current are in phase. For a capacitor, voltage lags current by **90°**. The total voltage is the vector sum: $V_T = V_R + V_C$. Capacitance is calculated using $C=\frac{1}{2\pi f X_c}$.

- **Method:**

  1. Connect the circuit.

  2. Measure voltage across the resistor ($V_R$), capacitor ($V_C$), and total voltage ($V$).

  3. Draw the vector triangle.

  4. Calculate Ohmic resistance ($R$), leakage resistance ($r$), capacitor reactance ($X_c$), and capacitance ($C$).

## التجربة الرابعة: سعة المكثف بالمتجهات (Capacitor by Vectors)

**الهدف:** إثبات أن الجهد الكلي هو المجموع الاتجاهي لجهد المقاومة والمكثف $V^2 = V_R^2 + V_C^2$.

| Trial | $V_R$ (Volts) | $V_C$ (Volts) | $V_{Total}$ (Volts) |
| :---: | :---: | :---: | :---: |
| 1 | 3.0 | 4.0 | 5.0 |
| 2 | 6.0 | 8.0 | 10.0 |
| 3 | 4.5 | 6.0 | 7.5 |

---

## 5. Determination of a Coil Inductance by Vectors Method

- **Aim:** Determination of a coil inductance by vectors method.

- **Tools:** AC power supply, Voltmeter, Coil, Resistor, Breadboard.

- **Theory:** In an RL circuit, total voltage is the vector sum: $V_T = V_R + V_L$. Voltage leads current by **90°** in a pure inductor. Leakage resistance ($r$) accounts for energy loss. Inductance is calculated via $L=\frac{X_L}{2\pi f}$.

- **Method:**

  1. Connect the circuit.

  2. Measure voltage across the resistor ($V_R$), inductor ($V_L$), and total voltage ($V$).

  3. Draw the vector triangle.

  4. Calculate resistance ($R$), leakage resistance ($r$), inductive reactance ($X_L$), and coil inductance ($L$).

## التجربة الخامسة: حث الملف بالمتجهات (Coil Inductance by Vectors)

**الهدف:** إيجاد المجموع الاتجاهي لجهد المقاومة والملف. (بإهمال المقاومة الداخلية للملف لتسهيل الأرقام المثالية).

| Trial | $V_R$ (Volts) | $V_{Coil}$ (Volts) | $V_{Total}$ (Volts) |
| :---: | :---: | :---: | :---: |
| 1 | 8.0 | 6.0 | 10.0 |
| 2 | 4.0 | 3.0 | 5.0 |
| 3 | 12.0 | 5.0 | 13.0 |

---

## 6. RLC Resonance in Series Circuits

- **Aim:** Demonstrate resonance phenomena in RLC circuits and determine the resonant frequency ($F_r$) and bandwidth (BW).

- **Tools:** Function generator, Resistors, Inductor, Capacitor, Ammeter, Voltmeter, Breadboard.

- **Theory:** Resonance occurs when inductive and capacitive reactances are equal ($X_L = X_C$) but 180° out of phase. Impedance becomes minimum ($Z = R$) and current becomes maximum ($I_{max} = V/R$). Resonant frequency is $F_r = \frac{1}{2\pi\sqrt{LC}}$. Bandwidth is the difference between upper and lower cut-off frequencies ($f_H - f_L$).

- **Method:**

  1. Connect the circuit and switch on the function generator.

  2. Record current ($I$) as frequency ($F$) changes.

  3. Plot $I$ vs $F$.

  4. Find $F_r$ from the graph and calculate $BW = F_H - F_L$.

## التجربة السادسة: الرنين في دوائر التوالي (RLC Resonance)

**الهدف:** إيجاد تردد الرنين $F_r$ الذي يكون عنده التيار أعلى ما يمكن. (بافتراض $F_r = 1000 Hz$).

| Frequency $F$ (Hz) | Current $I$ (mA) |
| :---: | :---: |
| 600 | 8.0 |
| 800 | 20.0 |
| 900 | 35.0 |
| 1000 | 50.0 | _(Resonance Peak)_ |
| 1100 | 35.0 |
| 1200 | 20.0 |
| 1400 | 8.0 |

---

## 7. Filters

- **Aim:** Calculate the cutoff frequency ($F_c$) in RC circuits for low and high pass filters, understand Gain ($G$), and calculate the Attenuation factor ($\alpha$).

- **Tools:** Function generator, Capacitor, Resistor, Breadboard, Oscilloscope.

- **Theory:** Filters pass specific frequency bands and attenuate others. A low-pass filter passes frequencies below $F_c$, and a high-pass filter passes frequencies above $F_c$. Cutoff occurs where $V_R = V_C$, giving $F_c = \frac{1}{2\pi RC}$. Gain (dB) is $20\log(V_{out}/V_{in})$. Attenuation $\alpha = 1 - G$.

- **Method:**

  1. Connect the low-pass filter circuit.

  2. Vary frequency and determine $V_{out}$ on the oscilloscope.

  3. Repeat for the high-pass filter circuit.

  4. Plot both curves together to find the intersection, which is the cutoff frequency ($F_c$).

## التجربة السابعة: المرشحات (Low & High Pass Filters)

**الهدف:** إيجاد تردد القطع $F_c$ (نقطة التقاطع). بافتراض أن جهد الدخول $V_{in} = 10V$ وتردد القطع $F_c = 1000 Hz$.

| Frequency $F$ (Hz) | Low-Pass $V_{out}$ (V) | High-Pass $V_{out}$ (V) |
| :---: | :---: | :---: |
| 100 | 9.95 | 1.00 |
| 500 | 8.94 | 4.47 |
| 1000 | 7.07 | 7.07 | _(Cutoff Frequency $F_c$)_ |
| 2000 | 4.47 | 8.94 |
| 10000 | 1.00 | 9.95 |

---

## 8. Clipper Circuits

- **Aim:** Understand clipping, graph the clipped signal vs the input signal, and calculate average value, RMS value, Form factor, and Ripple factor.

- **Tools:** AC Function generator, Digital oscilloscope, Diode, Resistor, Breadboard.

- **Theory:** Clipper (limiter) circuits remove a portion of an input signal without distorting the remaining waveform. A positive series clipper allows the negative half to pass while limiting the positive half, and vice versa for a negative clipper.

- **Method:**

  1. Connect the circuit.

  2. Set the input signal to a sine wave.

  3. Measure the output signal across the resistor using the oscilloscope.

  4. Measure maximum output value and calculate average, RMS, Form factor, and Ripple factor.

## التجربة الثامنة: دوائر القص (Clipper Circuits)

**الهدف:** حساب قيم الموجة المقصوصة (نصف موجة). بافتراض موجة دخل جيبية بجهد أقصى $V_m = 10V$.
_توضع هذه القيم كنتائج حسابية (Results) وليس كجدول متغيرات._

| Parameter                     | Formula              | Ideal Calculated Value |
| :---------------------------- | :------------------- | :--------------------- |
| **Max Input Voltage ($V_m$)** | Measured             | $10 V$                 |
| **Average Value ($V_{dc}$)**  | $V_m / \pi$          | $3.18 V$               |
| **RMS Value ($V_{rms}$)**     | $V_m / 2$            | $5.00 V$               |
| **Form Factor (F.F)**         | $V_{rms} / V_{dc}$   | $1.57$                 |
| **Ripple Factor ($\gamma$)**  | $\sqrt{(F.F)^2 - 1}$ | $1.21$                 |
