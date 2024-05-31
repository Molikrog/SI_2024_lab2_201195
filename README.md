# SI_2024_lab2_201195
Martin Simonoski
201195

2.
![SILab2_CFG](https://github.com/Molikrog/SI_2024_lab2_201195/assets/166874918/a22c7bf9-6b9b-4cac-994f-3b3d79e405e6)



3.
M = E - N + 2*P

M = 23 - 20 + 2

M = 5

4.

1.[allItems, payment] [allitems == null, payment = n] Ова е во случај ако од самиот почеток ако стигнеме на "null" поинтер каде фрламе "exception" за да престане програмата.
2.[item = allItems.get(i), payment, sum = 0] [item.getBarcode == null] Ова е уште еден "null" поинтер каде фрламе "exception" и се рестартира програмата после сменетата грешка 
3.[item = allItems.get(i), payment, sum = 0] [item.getBarcode != null] [chars = item.getBarcode.getArray][c = item.getBarcode().charAt()]
[allowed.indexOf(c) == -1]  Ова е уште еден "null" поинтер каде фрламе "exception" и се рестартира програмата после сменетата грешка
4. [item = allItems.get(i), payment, sum = 0] [item.getBarcode != null] [chars = item.getBarcode.getArray][c = item.getBarcode().charAt()]
[allowed.indexOf(c) != -1] [sum = item.getPrice()*items.getDiscount()][item.getPrice() > 300 && item.getDiscount() > 0 && item.getBarcode().charAt(0) == '0'][true] ова ќе е услов каде сите услови враќаат вистина и крајниот боолеан е true
5.[item = allItems.get(i), payment, sum = 0] [item.getBarcode != null] [chars = item.getBarcode.getArray][c = item.getBarcode().charAt()]
[allowed.indexOf(c) != -1] [sum = item.getPrice()*items.getDiscount()][item.getPrice() > 300 && item.getDiscount() > 0 && item.getBarcode().charAt(0) =! '0'][true] Овдека е каде во поглед на едниот услов е неточен ама само ја мења вредноста на сумата што не мора секад да значи на различен услов, сепак boolean може пак да врати вистина
6.[item = allItems.get(i), payment, sum = 0] [item.getBarcode != null] [chars = item.getBarcode.getArray][c = item.getBarcode().charAt()]
[allowed.indexOf(c) != -1] [sum = item.getPrice()][item.getPrice() > 300 && item.getDiscount() > 0 && item.getBarcode().charAt(0) == '0'][true] исто нешто како претходното само едниот услов не бил исполнет за дискаунтот и е вратено пак вистина
7.[item = allItems.get(i), payment, sum = 0] [item.getBarcode != null] [chars = item.getBarcode.getArray][c = item.getBarcode().charAt()]
[allowed.indexOf(c) != -1] [sum = item.getPrice()][item.getPrice() > 300 && item.getDiscount() > 0 && item.getBarcode().charAt(0) =! '0'][true] исто како претходните во услов каде немаат голема разлика условите сепак си е вистинито враќањето
8.[item = allItems.get(i), payment, sum = 0] [item.getBarcode != null] [chars = item.getBarcode.getArray][c = item.getBarcode().charAt()]
[allowed.indexOf(c) != -1] [sum = item.getPrice()*items.getDiscount()][item.getPrice() > 300 && item.getDiscount() > 0 && item.getBarcode().charAt(0) =! '0'][false] момент каде без разлика ако сите услови се исполнети сепак враќа грешка на корисникот бидејки самата сума е помала
9.[item = allItems.get(i), payment, sum = 0] [item.getBarcode != null] [chars = item.getBarcode.getArray][c = item.getBarcode().charAt()]
[allowed.indexOf(c) != -1] [sum = item.getPrice()*items.getDiscount()][item.getPrice() > 300 && item.getDiscount() > 0 && item.getBarcode().charAt(0) == '0'][false] момент каде без разлика ако сите услови се исполнети сепак враќа грешка на корисникот бидејки самата сума е помала, сепак треба да се премине низ целата програма и да се видат сите можни резултати
10.[item = allItems.get(i), payment, sum = 0] [item.getBarcode != null] [chars = item.getBarcode.getArray][c = item.getBarcode().charAt()]
[allowed.indexOf(c) != -1] [sum = item.getPrice()][item.getPrice() > 300 && item.getDiscount() > 0 && item.getBarcode().charAt(0) =! '0'][false] Ова е услов каде сите освен exceptions е грешно и испаѓа главното враќање да е исто погрешно

5.
1.[sum = item.getPrice()*items.getDiscount()][item.getPrice() > 300 && item.getDiscount() > 0 && item.getBarcode().charAt(0) == '0']
Бидејќи едини услов за да е вистин if условот е или сите да се точни имаме случај каде сите го исполнуваат и влага во вистинит if услов

2.[sum = item.getPrice()*items.getDiscount()][item.getPrice() > 300 && item.getDiscount() > 0 && item.getBarcode().charAt(0) == '0']
без разлика кое и да се избере ако не влезе во неважечки услов или item.getprice < 300, ќе мора да врати грешниот услов бидејќи се работи со &&.
