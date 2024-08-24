<h1>Тема: "Методы безусловной многомерной оптимизации"</h1>

> <strong><h2>Целевая функция</h2></strong>
> <p>f(x1, x2) = 101x1^2 - 200x1x2 + 101x2^2 - 94x1 - 7x2 + 53 </p>
> <strong><h2>Задание</h2></strong>
> <p>Построить таблицу для  x^(0) = (x1^(0); x2^(0)) = (1;1) и x^(0) = (x1^(0); x2^(0)) = (-1;-1) методами: 1)	Градиентный с постоянным шагом; 2)	Градиентный с дроблением шага; 3)	Метод наискорейшего спуска.</p>
> <p><strong>Найти точное решение</strong> (на основе необходимых условий минимума).</p>
> <p>В точке минимума функции должны выполняться необходимые условия первого порядка: в точке минимума частные производные первого порядка должны быть равны нулю.</p>

> <strong><h2>Выполнение задания:</h2></strong>
> <p>Вычислим частные производные первого порядка целевой функции по x1 и x2:</p>
> <p>∂f/(∂x1) = 202x1 - 200x2 - 94 = 0</p>
> <p>∂f/(∂x2) = -200x1 + 202x2 - 7 = 0</p>
> <p>Из первого уравнения выражаем x1:</p>
> <p>x1 = (200x2 + 94)/202</p>
> <p>И подставим во второе уравнение:</p>
> <p>-200 * ((200x2 + 94)/202) + 202x2 - 7 = 0</p>
> <p>x2 = 3369/134</p>
> <p>Отсюда:</p>
> <p>x1 = (200 * 3369/134 + 94)/202 = 1699/67</p>
> <p>Ответ:</p>
> <p>x1 = 1699/67 ≈ 25,35821</p>
> <p>x2 = 3369/134 ≈ 25,14179</p>

<strong>График функции</strong>

![image](https://github.com/user-attachments/assets/c2697891-513b-4de3-bb0a-15a111a0e60d)
<p>Рисунок 1 − График функции f(x1, x2) = 101x1^2 - 200x1x2 + 101x2^2 - 94x1 - 7x2 + 53</p> <br>
<strong>Расчетные таблицы при  x^(0) = (x1^(0); x2^(0)) = (1; 1):

<table width="0">
<tbody>
<tr>
<td colspan="9" width="652">
<p>Градиентный с дробленным шагом</p>
</td>
</tr>
<tr>
<td width="61">ɛ</td>
<td width="77">x1</td>
<td width="77">x2</td>
<td width="89">y</td>
<td width="115">Eфакт</td>
<td width="56">N</td>
<td width="65">N0</td>
<td width="56">N1</td>
<td width="56">
<p>l</p>
</td>
</tr>
<tr>
<td width="61">10^-1</td>
<td width="77">
<p>25,3229</p>
</td>
<td width="77">
<p>25,1065</p>
</td>
<td width="89">
<p>-1226,83</p>
</td>
<td width="115">
<p>0,0498649</p>
</td>
<td width="56">
<p>3338</p>
</td>
<td width="65">
<p>1672</p>
</td>
<td width="56">
<p>1666</p>
</td>
<td width="56">
<p>832</p>
</td>
</tr>
<tr>
<td width="61">10^-2</td>
<td width="77">
<p>25,3547</p>
</td>
<td width="77">
<p>25,1383</p>
</td>
<td width="89">
<p>-1226,83</p>
</td>
<td width="115">
<p>0,00497001</p>
</td>
<td width="56">
<p>4514</p>
</td>
<td width="65">
<p>2260</p>
</td>
<td width="56">
<p>2254</p>
</td>
<td width="56">
<p>1126</p>
</td>
</tr>
<tr>
<td width="61">10^-3</td>
<td width="77">
<p>25,3579</p>
</td>
<td width="77">
<p>25,1414</p>
</td>
<td width="89">
<p>-1226,83</p>
</td>
<td width="115">
<p>0,000499262</p>
</td>
<td width="56">
<p>5686</p>
</td>
<td width="65">
<p>2846</p>
</td>
<td width="56">
<p>2840</p>
</td>
<td width="56">
<p>1419</p>
</td>
</tr>
<tr>
<td width="61">10^-4</td>
<td width="77">
<p>25,3582</p>
</td>
<td width="77">
<p>25,1418</p>
</td>
<td width="89">
<p>-1226,83</p>
</td>
<td width="115">
<p>4,9783e-05</p>
</td>
<td width="56">
<p>6862</p>
</td>
<td width="65">
<p>3434</p>
</td>
<td width="56">
<p>3428</p>
</td>
<td width="56">
<p>1713</p>
</td>
</tr>
<tr>
<td width="61">10^-5</td>
<td width="77">
<p>&minus;</p>
</td>
<td width="77">
<p>&minus;</p>
</td>
<td width="89">
<p>&minus;</p>
</td>
<td width="115">
<p>&minus;</p>
</td>
<td width="56">
<p>&minus;</p>
</td>
<td width="65">
<p>&minus;</p>
</td>
<td width="56">
<p>&minus;</p>
</td>
<td width="56">
<p>&minus;</p>
</td>
</tr>
</tbody>
</table>


<table width="0">
<tbody>
<tr>
<td colspan="9" width="652">
<p>Градиентный с постоянным шагом</p>
</td>
</tr>
<tr>
<td width="61">ɛ</td>
<td width="77">x1</td>
<td width="77">x2</td>
<td width="89">y</td>
<td width="115">Eфакт</td>
<td width="56">N</td>
<td width="65">N0</td>
<td width="56">N1</td>
<td width="56">
<p>l</p>
</td>
</tr>
<tr>
<td width="61">10^-1</td>
<td width="77">
<p>25,3309</p>
</td>
<td width="77">
<p>25,1147</p>
</td>
<td width="89">
<p>-1226,83</p>
</td>
<td width="115">
<p>0,0384154</p>
</td>
<td width="56">
<p>1302</p>
</td>
<td width="64">
<p>0</p>
</td>
<td width="56">
<p>1302</p>
</td>
<td width="56">
<p>650</p>
</td>
</tr>
<tr>
<td width="61">10^-2</td>
<td width="77">
<p>25,3554</p>
</td>
<td width="77">
<p>25,139</p>
</td>
<td width="89">
<p>-1226,83</p>
</td>
<td width="115">
<p>0,00393039</p>
</td>
<td width="56">
<p>1738</p>
</td>
<td width="64">
<p>0</p>
</td>
<td width="56">
<p>1738</p>
</td>
<td width="56">
<p>868</p>
</td>
</tr>
<tr>
<td width="61">10^-3</td>
<td width="77">
<p>25,3579</p>
</td>
<td width="77">
<p>25,1415</p>
</td>
<td width="89">
<p>-1226,83</p>
</td>
<td width="115">
<p>0,000402137</p>
</td>
<td width="56">
<p>2174</p>
</td>
<td width="64">
<p>0</p>
</td>
<td width="56">
<p>2174</p>
</td>
<td width="56">
<p>1086</p>
</td>
</tr>
<tr>
<td width="61">10^-4</td>
<td width="77">
<p>25,3582</p>
</td>
<td width="77">
<p>25,1418</p>
</td>
<td width="89">
<p>-1226,83</p>
</td>
<td width="115">
<p>3,74379e-05</p>
</td>
<td width="56">
<p>2450</p>
</td>
<td width="64">
<p>0</p>
</td>
<td width="56">
<p>2450</p>
</td>
<td width="56">
<p>1224</p>
</td>
</tr>
<tr>
<td width="61">10^-5</td>
<td width="77">
<p>25,3582</p>
</td>
<td width="77">
<p>25,1418</p>
</td>
<td width="89">
<p>-1226,83</p>
</td>
<td width="115">
<p>4,53222e-06</p>
</td>
<td width="56">
<p>2642</p>
</td>
<td width="64">
<p>0</p>
</td>
<td width="56">
<p>2642</p>
</td>
<td width="56">
<p>1320</p>
</td>
</tr>
</tbody>
</table>


<table width="0">
<tbody>
<tr>
<td colspan="9" width="652">
<p>Наискорейший спуск</p>
</td>
</tr>
<tr>
<td width="61">ɛ</td>
<td width="77">x1</td>
<td width="77">x2</td>
<td width="89">y</td>
<td width="115">Eфакт</td>
<td width="56">N</td>
<td width="65">N0</td>
<td width="56">N1</td>
<td width="56">
<p>l</p>
</td>
</tr>
<tr>
<td width="61">10^-1</td>
<td width="77">
<p>25,3309</p>
</td>
<td width="77">
<p>25,1147</p>
</td>
<td width="89">
<p>-1332,83</p>
</td>
<td width="115">
<p>0,0384154</p>
</td>
<td width="56">
<p>1316</p>
</td>
<td width="64">
<p>14</p>
</td>
<td width="56">
<p>1302</p>
</td>
<td width="56">
<p>650</p>
</td>
</tr>
<tr>
<td width="61">10^-2</td>
<td width="77">
<p>25,3554</p>
</td>
<td width="77">
<p>25,139</p>
</td>
<td width="89">
<p>-1332,83</p>
</td>
<td width="115">
<p>0,00393039</p>
</td>
<td width="56">
<p>1752</p>
</td>
<td width="64">
<p>14</p>
</td>
<td width="56">
<p>1738</p>
</td>
<td width="56">
<p>868</p>
</td>
</tr>
<tr>
<td width="61">10^-3</td>
<td width="77">
<p>25,3579</p>
</td>
<td width="77">
<p>25,1415</p>
</td>
<td width="89">
<p>-1332,83</p>
</td>
<td width="115">
<p>0,000402137</p>
</td>
<td width="56">
<p>2188</p>
</td>
<td width="64">
<p>14</p>
</td>
<td width="56">
<p>2174</p>
</td>
<td width="56">
<p>1086</p>
</td>
</tr>
<tr>
<td width="61">10^-4</td>
<td width="77">
<p>25,3582</p>
</td>
<td width="77">
<p>25,1418</p>
</td>
<td width="89">
<p>-1332,83</p>
</td>
<td width="115">
<p>3,74379e-05</p>
</td>
<td width="56">
<p>2464</p>
</td>
<td width="64">
<p>14</p>
</td>
<td width="56">
<p>2450</p>
</td>
<td width="56">
<p>1224</p>
</td>
</tr>
<tr>
<td width="61">10^-5</td>
<td width="77">
<p>25,3582</p>
</td>
<td width="77">
<p>25,1418</p>
</td>
<td width="89">
<p>-1332,83</p>
</td>
<td width="115">
<p>4,53222e-06</p>
</td>
<td width="56">
<p>2656</p>
</td>
<td width="64">
<p>14</p>
</td>
<td width="56">
<p>2642</p>
</td>
<td width="56">
<p>1320</p>
</td>
</tr>
</tbody>
</table>

<strong>Расчетные таблицы при  x^(0) = (x1^(0); x2^(0)) = (-1; -1):
<table width="0">
<tbody>
<tr>
<td colspan="9" width="652">
<p>Градиентный с дробленным шагом</p>
</td>
</tr>
<tr>
<td width="61">ɛ</td>
<td width="77">x1</td>
<td width="77">x2</td>
<td width="89">y</td>
<td width="115">Eфакт</td>
<td width="56">N</td>
<td width="65">N0</td>
<td width="56">N1</td>
<td width="56">
<p>l</p>
</td>
</tr>
<tr>
<td width="61">10^-1</td>
<td width="77">
<p>25,3229</p>
</td>
<td width="77">
<p>25,1065</p>
</td>
<td width="89">
<p>-1226,83</p>
</td>
<td width="113">
<p>0,0499057</p>
</td>
<td width="56">
<p>3378</p>
</td>
<td width="65">
<p>1692</p>
</td>
<td width="56">
<p>1686</p>
</td>
<td width="56">
<p>842</p>
</td>
</tr>
<tr>
<td width="61">10^-2</td>
<td width="77">
<p>25,3547</p>
</td>
<td width="77">
<p>25,1383</p>
</td>
<td width="89">
<p>-1226,83</p>
</td>
<td width="113">
<p>0,00497408</p>
</td>
<td width="56">
<p>4554</p>
</td>
<td width="65">
<p>2280</p>
</td>
<td width="56">
<p>2274</p>
</td>
<td width="56">
<p>1136</p>
</td>
</tr>
<tr>
<td width="61">10^-3</td>
<td width="77">
<p>25,3579</p>
</td>
<td width="77">
<p>25,1414</p>
</td>
<td width="89">
<p>-1226,83</p>
</td>
<td width="113">
<p>0,00049967</p>
</td>
<td width="56">
<p>5726</p>
</td>
<td width="65">
<p>2866</p>
</td>
<td width="56">
<p>2860</p>
</td>
<td width="56">
<p>1429</p>
</td>
</tr>
<tr>
<td width="61">10^-4</td>
<td width="77">
<p>25,3582</p>
</td>
<td width="77">
<p>25,1418</p>
</td>
<td width="89">
<p>-1226,83</p>
</td>
<td width="113">
<p>4,98237e-05</p>
</td>
<td width="56">
<p>6902</p>
</td>
<td width="65">
<p>3454</p>
</td>
<td width="56">
<p>3448</p>
</td>
<td width="56">
<p>1723</p>
</td>
</tr>
<tr>
<td width="61">10^-5</td>
<td width="77">
<p>&minus;</p>
</td>
<td width="77">
<p>&minus;</p>
</td>
<td width="89">
<p>&minus;</p>
</td>
<td width="113">
<p>&minus;</p>
</td>
<td width="56">
<p>&minus;</p>
</td>
<td width="65">
<p>&minus;</p>
</td>
<td width="56">
<p>&minus;</p>
</td>
<td width="56">
<p>&minus;</p>
</td>
</tr>
</tbody>
</table>


<table width="0">
<tbody>
<tr>
<td colspan="9" width="652">
<p>Градиентный с постоянным шагом</p>
</td>
</tr>
<tr>
<td width="61">ɛ</td>
<td width="77">x1</td>
<td width="77">x2</td>
<td width="89">y</td>
<td width="115">Eфакт</td>
<td width="56">N</td>
<td width="65">N0</td>
<td width="56">N1</td>
<td width="56">
<p>l</p>
</td>
</tr>
<tr>
<td width="61">10^-1</td>
<td width="77">
<p>25,3298</p>
</td>
<td width="77">
<p>25,1132</p>
</td>
<td width="90">
<p>-1226,83</p>
</td>
<td width="113">
<p>0,0402867</p>
</td>
<td width="57">
<p>1308</p>
</td>
<td width="65">
<p>0</p>
</td>
<td width="57">
<p>1308</p>
</td>
<td width="56">
<p>653</p>
</td>
</tr>
<tr>
<td width="61">10^-2</td>
<td width="77">
<p>25,3554</p>
</td>
<td width="77">
<p>25,139</p>
</td>
<td width="90">
<p>-1226,83</p>
</td>
<td width="113">
<p>0,00391342</p>
</td>
<td width="57">
<p>1754</p>
</td>
<td width="65">
<p>0</p>
</td>
<td width="57">
<p>1754</p>
</td>
<td width="56">
<p>876</p>
</td>
</tr>
<tr>
<td width="61">10^-3</td>
<td width="77">
<p>25,3579</p>
</td>
<td width="77">
<p>25,1415</p>
</td>
<td width="90">
<p>-1226,83</p>
</td>
<td width="113">
<p>0,0004004</p>
</td>
<td width="57">
<p>2190</p>
</td>
<td width="65">
<p>0</p>
</td>
<td width="57">
<p>2190</p>
</td>
<td width="56">
<p>1094</p>
</td>
</tr>
<tr>
<td width="61">10^-4</td>
<td width="77">
<p>25,3582</p>
</td>
<td width="77">
<p>25,1418</p>
</td>
<td width="90">
<p>-1226,83</p>
</td>
<td width="113">
<p>4,6009e-05</p>
</td>
<td width="57">
<p>2478</p>
</td>
<td width="65">
<p>0</p>
</td>
<td width="57">
<p>2478</p>
</td>
<td width="56">
<p>1238</p>
</td>
</tr>
<tr>
<td width="61">10^-5</td>
<td width="77">
<p>25,3582</p>
</td>
<td width="77">
<p>25,1418</p>
</td>
<td width="90">
<p>-1226,83</p>
</td>
<td width="113">
<p>4,59392e-06</p>
</td>
<td width="57">
<p>2648</p>
</td>
<td width="65">
<p>0</p>
</td>
<td width="57">
<p>2648</p>
</td>
<td width="56">
<p>1323</p>
</td>
</tr>
</tbody>
</table>


<table width="0">
<tbody>
<tr>
<td colspan="9" width="652">
<p>Наискорейший спуск</p>
</td>
</tr>
<tr>
<td width="61">ɛ</td>
<td width="77">x1</td>
<td width="77">x2</td>
<td width="89">y</td>
<td width="115">Eфакт</td>
<td width="56">N</td>
<td width="65">N0</td>
<td width="56">N1</td>
<td width="56">
<p>l</p>
</td>
</tr>
<tr>
<td width="61">10^-1</td>
<td width="77">
<p>25,3298</p>
</td>
<td width="77">
<p>25,1132</p>
</td>
<td width="90">
<p>-1332,83</p>
</td>
<td width="113">
<p>0,0402867</p>
</td>
<td width="57">
<p>1322</p>
</td>
<td width="65">
<p>14</p>
</td>
<td width="57">
<p>1308</p>
</td>
<td width="56">
<p>653</p>
</td>
</tr>
<tr>
<td width="61">10^-2</td>
<td width="77">
<p>25,3554</p>
</td>
<td width="77">
<p>25,139</p>
</td>
<td width="90">
<p>-1332,83</p>
</td>
<td width="113">
<p>0,00391342</p>
</td>
<td width="57">
<p>1768</p>
</td>
<td width="65">
<p>14</p>
</td>
<td width="57">
<p>1754</p>
</td>
<td width="56">
<p>876</p>
</td>
</tr>
<tr>
<td width="61">10^-3</td>
<td width="77">
<p>25,3579</p>
</td>
<td width="77">
<p>25,1415</p>
</td>
<td width="90">
<p>-1332,83</p>
</td>
<td width="113">
<p>0,0004004</p>
</td>
<td width="57">
<p>2204</p>
</td>
<td width="65">
<p>14</p>
</td>
<td width="57">
<p>2190</p>
</td>
<td width="56">
<p>1094</p>
</td>
</tr>
<tr>
<td width="61">10^-4</td>
<td width="77">
<p>25,3582</p>
</td>
<td width="77">
<p>25,1418</p>
</td>
<td width="90">
<p>-1332,83</p>
</td>
<td width="113">
<p>4,6009e-05</p>
</td>
<td width="57">
<p>2492</p>
</td>
<td width="65">
<p>14</p>
</td>
<td width="57">
<p>2478</p>
</td>
<td width="56">
<p>1238</p>
</td>
</tr>
<tr>
<td width="61">10^-5</td>
<td width="77">
<p>25,3582</p>
</td>
<td width="77">
<p>25,1418</p>
</td>
<td width="90">
<p>-1332,83</p>
</td>
<td width="113">
<p>4,59392e-06</p>
</td>
<td width="57">
<p>2662</p>
</td>
<td width="65">
<p>14</p>
</td>
<td width="57">
<p>2648</p>
</td>
<td width="56">
<p>1323</p>
</td>
</tr>
</tbody>
</table>


<strong>Траектория движения точек при x^(0) = (x1^(0); x2^(0)) = (1; 1):

![image](https://github.com/user-attachments/assets/a338b280-420b-4ea5-afb8-199b25281557)
<p>Рисунок 2 − Градиентный с дробленным шагом</p>

![image](https://github.com/user-attachments/assets/6e003e2d-029b-412f-98ce-f12c6ec6edef)
<p>Рисунок 3 − Градиентный с постоянным шагом</p>

![image](https://github.com/user-attachments/assets/97e54a74-35bd-43bd-9f2d-c397d995af94)
<p>Рисунок 4 − Наискорейший спуск</p>

<strong>Траектория движения точек при x^(0) = (x1^(0); x2^(0)) = (-1; -1):

![image](https://github.com/user-attachments/assets/4b83749b-86a6-408d-8c88-ac9506839d9e)
<p>Рисунок 5 − Градиентный с дробленным шагом</p>

![image](https://github.com/user-attachments/assets/30b33065-68f5-4168-9bc2-5609fc4ba59f)
<p>Рисунок 6 − Градиентный с постоянным шагом</p>

![image](https://github.com/user-attachments/assets/96a66a75-7964-4058-a0eb-82927a7d156d)
<p>Рисунок 7 − Наискорейший спуск</p>

<p><strong>Вывод:</strong> в ходе выполнения данной лабораторной работы были сравнены градиентные методы (градиентный метод с дроблением шага; градиентный метод с постоянным шагом; метод наискорейшего спуска). Лучшим методом оказался метод наискорейшего спуска, для заданной целевой функции и для заданных условий окончания поиска по критерию минимального числа экспериментов. </p><br>
