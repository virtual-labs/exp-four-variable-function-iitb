In Experiment # 1 we studied the use of IC 74LS153 as a Dual 4:1 MUX. We required only one IC 74LS153 to design an 8:1 MUX. Now in Experiment # 2 we shall study the application of MUX as a Universal Logic Generator for a four variable system.&nbsp;<br />
To implement a four variable Universal Function Generator using IC 74LS153, let us follow these steps:<br />
1.&nbsp;&nbsp; &nbsp;To begin with we shall design a 16:1 MUX using multiple 74LS153 ICs.&nbsp;<br />
2.&nbsp;&nbsp; &nbsp;IC 74LS153 has two 4:1 MUXes within it. Each MUX has two select lines and four data input lines. So in all eight data inputs D0 to D7 are available from first IC # U1.<br />
3.&nbsp;&nbsp; &nbsp;Similarly second IC # U2 provides another eight data inputs D8 to D15. Thus in all 16 input lines are now available.<br />
4.&nbsp;&nbsp; &nbsp;To select one of these 16 data inputs, we need four select lines; let us label them as A B C &amp; D; where A is the most significant bit (MSB) and D is the least significant bit (LSB).&nbsp;<br />
5.&nbsp;&nbsp; &nbsp;Each IC has 4 select lines.&nbsp;<br />
6.&nbsp;&nbsp; &nbsp;All eight select lines of U1 and U2 are connected together and labelled as select lines C &amp; D. &nbsp;<br />
7.&nbsp;&nbsp; &nbsp;To get additional two select lines we introduce the third IC U3. Only one 4:1 MUX of U3 is required. The two select lines of U3 are labelled as A &amp; B.&nbsp;<br />
8.&nbsp;&nbsp; &nbsp;The strobe inputs 1G&rsquo; &amp; 2G&rsquo; of all the ICs is connected to ground so that all the IC&rsquo;s are enabled for operation.<br />
9.&nbsp;&nbsp; &nbsp;Thus in all we need three IC&rsquo;s for the design of 4-variable Universal Logic Generator as shown in Fig.1.<br />
The output function F can be written as:<br />
F = A&rsquo;.B&rsquo;.Y0 + A&rsquo;.B.Y1 +A.B&rsquo;.Y2 +A.B.Y3

<center>
<img src="images/image001.png">
<br/>Fig.1. Four variable - Universal Logic Function Generator<br />
</center>

<span ><span >The function table for Fig.1 is given below. Any four variable logic function can be derived using this circuit.</span></span>
<br/><center>
<div>
<table border="1" cellspacing="0" class="MsoTableGrid" >
	<tbody>
		<tr>
			<td>
			<p ><span ><span >Decimal</span></span></p>
			</td>
			<td colspan="4">
			<p ><span ><span>Select Lines</span></span></p>
			</td>
			<td>
			<p ><span ><span>Output</span></span></p>
			</td>
		</tr>
		<tr>
			<td>
			<p ><span ><span>Equivalent</span></span></p>
			</td>
			<td>
			<p ><strong><span ><span>A</span></span></strong></p>
			</td>
			<td>
			<p ><strong><span ><span>B</span></span></strong></p>
			</td>
			<td>
			<p ><strong><span ><span>C</span></span></strong></p>
			</td>
			<td>
			<p ><strong><span ><span>D</span></span></strong></p>
			</td>
			<td>
			<p ><strong><span ><span>Y</span></span></strong></p>
			</td>
		</tr>
		<tr>
			<td>
			<p ><span ><span>0</span></span></p>
			</td>
			<td>
			<p ><span ><span>0</span></span></p>
			</td>
			<td>
			<p ><span ><span>0</span></span></p>
			</td>
			<td>
			<p ><span ><span>0</span></span></p>
			</td>
			<td>
			<p ><span ><span>0</span></span></p>
			</td>
			<td>
			<p ><span ><span>D0</span></span></p>
			</td>
		</tr>
		<tr>
			<td>
			<p ><span ><span>1</span></span></p>
			</td>
			<td>
			<p ><span ><span>0</span></span></p>
			</td>
			<td>
			<p ><span ><span>0</span></span></p>
			</td>
			<td>
			<p ><span ><span>0</span></span></p>
			</td>
			<td>
			<p ><span ><span>1</span></span></p>
			</td>
			<td>
			<p ><span ><span>D1</span></span></p>
			</td>
		</tr>
		<tr>
			<td>
			<p ><span ><span>2</span></span></p>
			</td>
			<td>
			<p ><span ><span>0</span></span></p>
			</td>
			<td>
			<p ><span ><span>0</span></span></p>
			</td>
			<td>
			<p ><span ><span>1</span></span></p>
			</td>
			<td>
			<p ><span ><span>0</span></span></p>
			</td>
			<td>
			<p ><span ><span>D2</span></span></p>
			</td>
		</tr>
		<tr>
			<td>
			<p ><span ><span>3</span></span></p>
			</td>
			<td>
			<p ><span ><span>0</span></span></p>
			</td>
			<td>
			<p ><span ><span>0</span></span></p>
			</td>
			<td>
			<p ><span ><span>1</span></span></p>
			</td>
			<td>
			<p ><span ><span>1</span></span></p>
			</td>
			<td>
			<p ><span ><span>D3</span></span></p>
			</td>
		</tr>
		<tr>
			<td>
			<p ><span ><span>4</span></span></p>
			</td>
			<td>
			<p ><span ><span>0</span></span></p>
			</td>
			<td>
			<p ><span ><span>1</span></span></p>
			</td>
			<td>
			<p ><span ><span>0</span></span></p>
			</td>
			<td>
			<p ><span ><span>0</span></span></p>
			</td>
			<td>
			<p ><span ><span>D4</span></span></p>
			</td>
		</tr>
		<tr>
			<td>
			<p ><span ><span>5</span></span></p>
			</td>
			<td>
			<p ><span ><span>0</span></span></p>
			</td>
			<td>
			<p ><span ><span>1</span></span></p>
			</td>
			<td>
			<p ><span ><span>0</span></span></p>
			</td>
			<td>
			<p ><span ><span>1</span></span></p>
			</td>
			<td>
			<p ><span ><span>D5</span></span></p>
			</td>
		</tr>
		<tr>
			<td>
			<p ><span ><span>6</span></span></p>
			</td>
			<td>
			<p ><span ><span>0</span></span></p>
			</td>
			<td>
			<p ><span ><span>1</span></span></p>
			</td>
			<td>
			<p ><span ><span>1</span></span></p>
			</td>
			<td>
			<p ><span ><span>0</span></span></p>
			</td>
			<td>
			<p ><span ><span>D6</span></span></p>
			</td>
		</tr>
		<tr>
			<td>
			<p ><span ><span>7</span></span></p>
			</td>
			<td>
			<p ><span ><span>0</span></span></p>
			</td>
			<td>
			<p ><span ><span>1</span></span></p>
			</td>
			<td>
			<p ><span ><span>1</span></span></p>
			</td>
			<td>
			<p ><span ><span>1</span></span></p>
			</td>
			<td>
			<p ><span ><span>D7</span></span></p>
			</td>
		</tr>
		<tr>
			<td>
			<p ><span ><span>8</span></span></p>
			</td>
			<td>
			<p><span ><span>1</span></span></p>
			</td>
			<td>
			<p ><span ><span>0</span></span></p>
			</td>
			<td>
			<p ><span ><span>0</span></span></p>
			</td>
			<td>
			<p ><span ><span>0</span></span></p>
			</td>
			<td>
			<p ><span ><span>D8</span></span></p>
			</td>
		</tr>
		<tr>
			<td>
			<p ><span ><span>9</span></span></p>
			</td>
			<td>
			<p><span ><span>1</span></span></p>
			</td>
			<td>
			<p ><span ><span>0</span></span></p>
			</td>
			<td>
			<p ><span ><span>0</span></span></p>
			</td>
			<td>
			<p ><span ><span>1</span></span></p>
			</td>
			<td>
			<p ><span ><span>D9</span></span></p>
			</td>
		</tr>
		<tr>
			<td>
			<p ><span ><span>10</span></span></p>
			</td>
			<td>
			<p><span ><span>1</span></span></p>
			</td>
			<td>
			<p ><span ><span>0</span></span></p>
			</td>
			<td>
			<p ><span ><span>1</span></span></p>
			</td>
			<td>
			<p ><span ><span>0</span></span></p>
			</td>
			<td>
			<p ><span ><span>D10</span></span></p>
			</td>
		</tr>
		<tr>
			<td>
			<p ><span ><span>11</span></span></p>
			</td>
			<td>
			<p><span ><span>1</span></span></p>
			</td>
			<td>
			<p ><span ><span>0</span></span></p>
			</td>
			<td>
			<p ><span ><span>1</span></span></p>
			</td>
			<td>
			<p ><span ><span>1</span></span></p>
			</td>
			<td>
			<p ><span ><span>D11</span></span></p>
			</td>
		</tr>
		<tr>
			<td>
			<p ><span ><span>12</span></span></p>
			</td>
			<td>
			<p><span ><span>1</span></span></p>
			</td>
			<td>
			<p ><span ><span>1</span></span></p>
			</td>
			<td>
			<p ><span ><span>0</span></span></p>
			</td>
			<td>
			<p ><span ><span>0</span></span></p>
			</td>
			<td>
			<p ><span ><span>D12</span></span></p>
			</td>
		</tr>
		<tr>
			<td>
			<p ><span ><span>13</span></span></p>
			</td>
			<td>
			<p><span ><span>1</span></span></p>
			</td>
			<td>
			<p ><span ><span>1</span></span></p>
			</td>
			<td>
			<p ><span ><span>0</span></span></p>
			</td>
			<td>
			<p ><span ><span>1</span></span></p>
			</td>
			<td>
			<p ><span ><span>D13</span></span></p>
			</td>
		</tr>
		<tr>
			<td>
			<p ><span ><span>14</span></span></p>
			</td>
			<td>
			<p><span ><span>1</span></span></p>
			</td>
			<td>
			<p ><span ><span>1</span></span></p>
			</td>
			<td>
			<p ><span ><span>1</span></span></p>
			</td>
			<td>
			<p ><span ><span>0</span></span></p>
			</td>
			<td>
			<p ><span ><span>D14</span></span></p>
			</td>
		</tr>
		<tr>
			<td>
			<p ><span ><span>15</span></span></p>
			</td>
			<td>
			<p><span ><span>1</span></span></p>
			</td>
			<td>
			<p ><span ><span>1</span></span></p>
			</td>
			<td>
			<p ><span ><span>1</span></span></p>
			</td>
			<td>
			<p ><span ><span>1</span></span></p>
			</td>
			<td>
			<p ><span ><span>D15</span></span></p>
			</td>
		</tr>
	</tbody>
</table>
</div>
</center><br/>
<div><span ><span>For the logic diagram &amp; pin diagram, refer Fig.2.&nbsp; The function table for IC 74LS153 is also provided for reference.</span></span></div>


<center>
<img src="images/image002.jpg">
<br/>Fig. 2. Internal Structure & Pin Diagram of IC74LS153<br /></center>
<br/>
<center>
<img src="images/image003.jpg"><br/>
<br/><img src="images/image004.png">
<br/>Fig. 3.Function Table<br /></center>

#### Numerical:

In 4-variable function, there are 4 select lines i.e. total 16 inputs (2<sup>4</sup> = 16).<br/><br/>
<div >
			<table>
				<tr>
					<th colspan=4>Select Lines</th>
					<th colspan=16>Inputs</th>
					<th>Output</th>
				</tr>
				<tr>
					<th>A</th>
					<th>B</th>
					<th>C</th>
					<th>D</th>
					<th>D0</th>
					<th>D1</th>
					<th>D2</th>
					<th>D3</th>
					<th>D4</th>
					<th>D5</th>
					<th>D6</th>
					<th>D7</th>
					<th>D8</th>
					<th>D9</th>
					<th>D10</th>
					<th>D11</th>
					<th>D12</th>
					<th>D13</th>
					<th>D14</th>
					<th>D15</th>
					<th>Y</th>
				</tr>
				<tr>
					<td>0</td>
					<td>0</td>
					<td>0</td>
					<td>0</td>
					<td>0</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>0</td>
				</tr>
				<tr>
					<td>0</td>
					<td>0</td>
					<td>0</td>
					<td>0</td>
					<td>1</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>1</td>
				</tr>
				<tr>
					<td>0</td>
					<td>0</td>
					<td>0</td>
					<td>1</td>
					<td>X</td>
					<td>0</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>0</td>
				</tr>
				<tr>
					<td>0</td>
					<td>0</td>
					<td>0</td>
					<td>1</td>
					<td>X</td>
					<td>1</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>1</td>
				</tr>
				<tr>
					<td>0</td>
					<td>0</td>
					<td>1</td>
					<td>0</td>
					<td>X</td>
					<td>X</td>
					<td>0</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>0</td>
				</tr>
				<tr>
					<td>0</td>
					<td>0</td>
					<td>1</td>
					<td>0</td>
					<td>X</td>
					<td>X</td>
					<td>1</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>1</td>
				</tr>
				<tr>
					<td>0</td>
					<td>0</td>
					<td>1</td>
					<td>1</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>0</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>0</td>
				</tr>
				<tr>
					<td>0</td>
					<td>0</td>
					<td>1</td>
					<td>1</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>1</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>1</td>
				</tr>
				<tr>
					<td>0</td>
					<td>1</td>
					<td>0</td>
					<td>0</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>0</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>0</td>
				</tr>
				<tr>
					<td>0</td>
					<td>1</td>
					<td>0</td>
					<td>0</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>1</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>1</td>
				</tr>
				<tr>
					<td>0</td>
					<td>1</td>
					<td>0</td>
					<td>1</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>0</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>0</td>
				</tr>
				<tr>
					<td>0</td>
					<td>1</td>
					<td>0</td>
					<td>1</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>1</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>1</td>
				</tr>
				<tr>
					<td>0</td>
					<td>1</td>
					<td>1</td>
					<td>0</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>0</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>0</td>
				</tr>
				<tr>
					<td>0</td>
					<td>1</td>
					<td>1</td>
					<td>0</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>1</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>1</td>
				</tr>
				<tr>
					<td>0</td>
					<td>1</td>
					<td>1</td>
					<td>1</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>0</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>0</td>
				</tr>
				<tr>
					<td>0</td>
					<td>1</td>
					<td>1</td>
					<td>1</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>1</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>1</td>
				</tr>
				<tr>
					<td>1</td>
					<td>0</td>
					<td>0</td>
					<td>0</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>0</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>0</td>
				</tr>
				<tr>
					<td>1</td>
					<td>0</td>
					<td>0</td>
					<td>0</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>1</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>1</td>
				</tr>
				<tr>
					<td>1</td>
					<td>0</td>
					<td>0</td>
					<td>1</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>0</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>0</td>
				</tr>
				<tr>
					<td>1</td>
					<td>0</td>
					<td>0</td>
					<td>1</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>1</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>1</td>
				</tr>
				<tr>
					<td>1</td>
					<td>0</td>
					<td>1</td>
					<td>0</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>0</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>0</td>
				</tr>
				<tr>
					<td>1</td>
					<td>0</td>
					<td>1</td>
					<td>0</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>1</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>1</td>
				</tr>
				<tr>
					<td>1</td>
					<td>0</td>
					<td>1</td>
					<td>1</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>0</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>0</td>
				</tr>
				<tr>
					<td>1</td>
					<td>0</td>
					<td>1</td>
					<td>1</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>1</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>1</td>
				</tr>
				<tr>
					<td>1</td>
					<td>1</td>
					<td>0</td>
					<td>0</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>0</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>0</td>
				</tr>
				<tr>
					<td>1</td>
					<td>1</td>
					<td>0</td>
					<td>0</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>1</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>1</td>
				</tr>
				<tr>
					<td>1</td>
					<td>1</td>
					<td>0</td>
					<td>1</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>0</td>
					<td>X</td>
					<td>X</td>
					<td>0</td>
				</tr>
				<tr>
					<td>1</td>
					<td>1</td>
					<td>0</td>
					<td>1</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>1</td>
					<td>X</td>
					<td>X</td>
					<td>1</td>
				</tr>
				<tr>
					<td>1</td>
					<td>1</td>
					<td>1</td>
					<td>0</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>0</td>
					<td>X</td>
					<td>0</td>
				</tr>
				<tr>
					<td>1</td>
					<td>1</td>
					<td>1</td>
					<td>0</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>1</td>
					<td>X</td>
					<td>1</td>
				</tr>
				<tr>
					<td>1</td>
					<td>1</td>
					<td>1</td>
					<td>1</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>0</td>
					<td>0</td>
				</tr>
				<tr>
					<td>1</td>
					<td>1</td>
					<td>1</td>
					<td>1</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>X</td>
					<td>1</td>
					<td>1</td>
				</tr>
			</table>
		</div>
		<br/>
		(Where : &lsquo;1&rsquo; indicate VCC/+5V,&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &lsquo;0&rsquo; indicate 0V, &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&lsquo;X&rsquo; indicate &ldquo;don&rsquo;t care&ldquo;)<br>

Here we have implemented <img src="images/nu_image001.png"> :-
<br/>&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; D0, D2, D4, D6, D8, D10, D12, D13&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; to&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; GND(Ground) <br/>
		&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;and&nbsp;&nbsp;&nbsp; D1, D3, D5, D7, D9, D11, D14, D15&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; to&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; VCC(+5V)<br/>

<br/>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;So the resultant truth table is :
<br/>
<div >
			<table>
				<tr>
					<th colspan=4>Inputs</th>
					<th>Output</th>
				</tr>
				<tr>
					<th>A</th>
					<th>B</th>
					<th>C</th>
					<th>D</th>
					<th>Y</th>
				</tr>
				<tr>
					<td>0</td>
					<td>0</td>
					<td>0</td>
					<td>0</td>
					<td>1</td>
				</tr>
				<tr>
					<td>0</td>
					<td>0</td>
					<td>0</td>
					<td>1</td>
					<td>0</td>
				</tr>
				<tr>
					<td>0</td>
					<td>0</td>
					<td>1</td>
					<td>0</td>
					<td>1</td>
				</tr>
				<tr>
					<td>0</td>
					<td>0</td>
					<td>1</td>
					<td>1</td>
					<td>0</td>
				</tr>
				<tr>
					<td>0</td>
					<td>1</td>
					<td>0</td>
					<td>0</td>
					<td>1</td>
				</tr>
				<tr>
					<td>0</td>
					<td>1</td>
					<td>0</td>
					<td>1</td>
					<td>0</td>
				</tr>
				<tr>
					<td>0</td>
					<td>1</td>
					<td>1</td>
					<td>0</td>
					<td>1</td>
				</tr>
				<tr>
					<td>0</td>
					<td>1</td>
					<td>1</td>
					<td>1</td>
					<td>0</td>
				</tr>
				<tr>
					<td>1</td>
					<td>0</td>
					<td>0</td>
					<td>0</td>
					<td>1</td>
				</tr>
				<tr>
					<td>1</td>
					<td>0</td>
					<td>0</td>
					<td>1</td>
					<td>0</td>
				</tr>
				<tr>
					<td>1</td>
					<td>0</td>
					<td>1</td>
					<td>0</td>
					<td>1</td>
				</tr>
				<tr>
					<td>1</td>
					<td>0</td>
					<td>1</td>
					<td>1</td>
					<td>0</td>
				</tr>
				<tr>
					<td>1</td>
					<td>1</td>
					<td>0</td>
					<td>0</td>
					<td>1</td>
				</tr>
				<tr>
					<td>1</td>
					<td>1</td>
					<td>0</td>
					<td>1</td>
					<td>1</td>
				</tr>
				<tr>
					<td>1</td>
					<td>1</td>
					<td>1</td>
					<td>0</td>
					<td>0</td>
				</tr>
				<tr>
					<td>1</td>
					<td>1</td>
					<td>1</td>
					<td>1</td>
					<td>0</td>
				</tr>
			</table>
	</div>

<script type="text/javascript" id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"> </script>