Download Link: https://assignmentchef.com/product/solved-csie-mini-programming-homework-1
<br>



<h1>Ada’s Demo Album</h1>

<h2>Problem Description</h2>

Ada, a CSIE student, is also an amateur songwriter. She recently writes a wonderful song consisting of <em>N </em>bars. To make this song more popular, she decides to cooperate with a record label.

In order to obtain a recording contract, she has to prepare a demo and submit it to a record label in hopes of being invited to record a full-length album in a professional recording studio. However, as a CSIE sophomore tortured by exploding assignments, she has no time to record an additional demo. Instead, she would like to simply submit a snatch of her <em>N</em>-barred song as a demo. A snatch of a song is valid if both the two following conditions hold:

<ul>

 <li>It can be obtained by removing several (possibly zero) bars from the beginning and several (possibly zero) bars from the end.</li>

 <li>It consists of at least 2 bars.</li>

</ul>

Before making an official submission, she has done some surveys in order to pick and present the best snatch to the record label. With valuable feedbacks and a statistical transformation, for the <em>i</em>-th bar (1 ≤ <em>i </em>≤ <em>N</em>), its greatness can be specified with a value <em>a<sub>i</sub></em>. Note that though Ada’s song is wonderful, <em>a<sub>i </sub></em>may be non-positive since a statistical transformation has been applied.

Fortunately, Ada also knows how a demo is rated in a record label. As humans are biased, the first impression and the ending of a demo may weigh differently in one’s mind. More specifically, given <em>x,y,z </em>from the record label, if the <em>`</em>-th bar, (<em>` </em>+ 1)-th bar, <em>…</em>, and the <em>r</em>-th bar of the song are submitted as the demo, its rating will be

Please help Ada determine which snatch should be picked to achieve the maximal rating.

<h2>Input</h2>

The first line of the input contains 4 integers <em>N</em>, <em>x</em>, <em>y</em>, <em>z</em>, denoting the number of bars in the original song and the coefficients used in rating evaluation.

The second line of the input contains <em>N </em>space-separated integers <em>a</em><sub>1</sub><em>,a</em><sub>2</sub><em>,…,a<sub>N</sub></em>, where the <em>i</em>-th integer denotes that greatness of the <em>i</em>-th bar.

<ul>

 <li>2 ≤ <em>N </em>≤ 2 × 10<sup>5</sup></li>

 <li>1 ≤ <em>x,y,z </em>≤ 10<sup>4</sup></li>

 <li>−10<sup>9 </sup>≤ <em>a<sub>i </sub></em>≤ 10<sup>9</sup><em>,</em>∀<em>i </em>= 1<em>,</em>2<em>,…,N</em></li>

</ul>

<table width="527">

 <tbody>

  <tr>

   <td width="328"><strong>Test Group 0 (0 %)</strong>•   Sample Input<strong>Test Group 2 (40 %)</strong>•   <em>x </em>= <em>y </em>= <em>z</em></td>

   <td width="199"><strong>Test Group 1 (10 %)</strong>•   <em>N </em>≤ 2000<strong>Test Group 3 (50 %)</strong>•   No Additional Constraint</td>

  </tr>

 </tbody>

</table>

<h2>Output</h2>

Please output an integer <em>S </em>indicating the maximal achievable rating.

<strong>Sample Input 1                            Sample Input 2                           Sample Input 3</strong>

6 1 1 1                                              8 59 4 87                                         3 5358 5926 3141

-12 7 -127 -1 -2 -7                                 0 8 -7 0 5 0 -2 9                            1 10000 100000000

<strong>Sample Output 1                          Sample Output 2                        Sample Output 3</strong>

-3                                                    1239                                               314159265358

<h2>Explanation</h2>

<ul>

 <li>In the first testcase, <em>S </em>achieves its maximum by taking (<em>`,r</em>) = (4<em>,</em>5), <em>S </em>= 1 · (−1) + 1 · (−2) = −3.</li>

 <li>In the second testcase, <em>S </em>achieves its maximum by taking (<em>`,r</em>) = (2<em>,</em>8), <em>S </em>= 59 · 8 + 4 · ((−7) + 0 + 5 + (−2)) + 87 · 9 = 1239.</li>

 <li>In the third testcase, <em>S </em>achieves its maximum by taking (<em>`,r</em>) = (1<em>,</em>3), <em>S </em>= 5358 · 1 + 5926 · 10<sup>4 </sup>+ 3141 · 10<sup>8 </sup>= 314159265358.</li>

</ul>

<h2>Hint</h2>

Roses are red,

Violets are blue,

See the Test Group 2?

It’s a d´ej`a vu.