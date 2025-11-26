---
{"dg-publish":true,"permalink":"/modelling-project/","tags":["gardenEntry"]}
---


# - How to get more accurate readings

- ## Zoomed in experiment
ممكن نجيب نفس ال exp و نعمل زوم علي مدة زمنية في الاول عشان نظبط ال Time rise و ال Time peak و نظبط ال parameters بحيث تجيب ال constants صح

معرفش لسا ازاي بس هنعمل كدا
- ## Multiple experiment running in parallel
 كذا قراية, كذا scenario, هنعمل كذا experiment في ال parameter estimation و نعملهم كلهم Use for Estimation و كدا هيظبطها و هيخليها ادق اكتر
 
- ## Tweaking Optimization parameters
mmkn n8er el tolerances and the optimization algorithms for more accurate iterations

- ## MUST model friction in mathematical model

- ممكن نعمل measurements لكل component لوحده عشان نظبط ال model, يعني علي الصورة التحت ممكن نقيس سرعة الماتور لوحده من غير حاجة عليه عشان نجيبله كل حاجة ليه و نستخدمها بقا في ال موديل الكبير, دا هيبقى ادق و اسرع و هيقلل iterations في ال exp الكبيرة

- ## In the SIMULINK model, we can enter a block named [ **Dead Zone** ] which will make the readings more accuarte, to get the dead zone we:

		1. Enter 0 into PWM
		2. Ramp up the PWM (Values range from 0 to 255) Till the motor starts Moving
		3. Let's say the motor started moving from 70 and upwards, the deadzone block would have the values 0 to 70 as a deadzone [NO LOAD]
		4. After adding the load, and retrying the experiment, we'll find the deadzone to be a higher number, say 120, the extra 50 levels is from mechanical friction
		5. The 50 levels on the PWM on arduino corosponds to a certian voltage level, we can know how much current it takes to overcome the friction

$V=\frac{i}{Ra}$ , $V*Ra =i$ , $Torque = Kt*i$ 
and from torque we can know how much force in newtons friction in our system is
$F = Torque / R_P$      -> Rp is Radius of pulley

>[!tip] we do not have Back emf here since we are testing deadzone, meaning we have current but no working motor rpm


		6. If we can test or measure ANY paramter before estimating it, measuring it before hand and lowering the amount of paramters to estimate is 100% better
		7. if the testing or measurment wont be 100% accurate, then the measurement would be used as a starting value for the estimator, still being helpful



>[!tip] Having the deadzone **KNOWN** in the model before hand allows the parameter estimator to work better with more accuracy.


- 

---




# - Physical model (?)

![PhysicalModelAIGen.png| 400](/img/user/PhysicalModelAIGen.png)

<p align='center' style="font-size: 1.5em;"> Generated using AI </p>
 بس حاسسها كويسة و بسيطة و سهلة كفاية ان احنا نعملها و مش هيبقى في عوامل كتيرة تاثر علينا في الحسابات و الموديل دا حساباته سهله
[[How to use obsidian\|How to use obsidian]]