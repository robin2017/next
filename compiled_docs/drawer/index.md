{"meta":"<h2 id=\"&#x4F7F;&#x7528;&#x6307;&#x5357;\">&#x4F7F;&#x7528;&#x6307;&#x5357;<a href=\"#&#x4F7F;&#x7528;&#x6307;&#x5357;\" class=\"anchor\">#</a></h2><p>&#x62BD;&#x5C49;</p>\n<h3 id=\"&#x4F55;&#x65F6;&#x4F7F;&#x7528;\">&#x4F55;&#x65F6;&#x4F7F;&#x7528;<a href=\"#&#x4F55;&#x65F6;&#x4F7F;&#x7528;\" class=\"anchor\">#</a></h3><p>&#x62BD;&#x5C49;&#x662F;&#x7528;&#x4E8E;&#x5728;&#x4E0D;&#x79BB;&#x5F00;&#x4E3B;&#x8DEF;&#x5F84;&#x7684;&#x60C5;&#x51B5;&#x4E0B;&#xFF0C;&#x63D0;&#x4F9B;&#x7528;&#x6237;&#x5FEB;&#x901F;&#x6267;&#x884C;&#x7B80;&#x5355;&#x7684;&#x64CD;&#x4F5C;&#x3001;&#x786E;&#x8BA4;&#x7528;&#x6237;&#x4FE1;&#x606F;&#x6216;&#x53CD;&#x9988;&#x63D0;&#x793A;&#x7684;&#x8F85;&#x52A9;&#x7A97;&#x53E3;&#x3002;</p>\n<h2 id=\"api\">API<a href=\"#api\" class=\"anchor\">#</a></h2>","api":"<h3 id=\"drawer\">Drawer<a href=\"#drawer\" class=\"anchor\">#</a></h3><table>\n<thead>\n<tr>\n<th>&#x53C2;&#x6570;</th>\n<th>&#x8BF4;&#x660E;</th>\n<th>&#x7C7B;&#x578B;</th>\n<th>&#x9ED8;&#x8BA4;&#x503C;</th>\n</tr>\n</thead>\n<tbody>\n<tr>\n<td>trigger</td>\n<td>&#x89E6;&#x53D1;&#x5F39;&#x5C42;&#x663E;&#x793A;&#x6216;&#x9690;&#x85CF;&#x7684;&#x5143;&#x7D20;</td>\n<td>ReactElement</td>\n<td>null</td>\n</tr>\n<tr>\n<td>triggerType</td>\n<td>&#x89E6;&#x53D1;&#x5F39;&#x5C42;&#x663E;&#x793A;&#x6216;&#x9690;&#x85CF;&#x7684;&#x64CD;&#x4F5C;&#x7C7B;&#x578B;&#xFF0C;&#x53EF;&#x4EE5;&#x662F; &apos;click&apos;&#xFF0C;&apos;hover&apos;&#xFF0C;&apos;focus&apos;&#xFF0C;&#x6216;&#x8005;&#x5B83;&#x4EEC;&#x7EC4;&#x6210;&#x7684;&#x6570;&#x7EC4;&#xFF0C;&#x5982; [&apos;hover&apos;, &apos;focus&apos;]</td>\n<td>String/Array</td>\n<td>&apos;click&apos;</td>\n</tr>\n<tr>\n<td>visible</td>\n<td>&#x662F;&#x5426;&#x663E;&#x793A;</td>\n<td>Boolean</td>\n<td>-</td>\n</tr>\n<tr>\n<td>hasMask</td>\n<td>&#x662F;&#x5426;&#x663E;&#x793A;&#x906E;&#x7F69;</td>\n<td>Boolean</td>\n<td>true</td>\n</tr>\n<tr>\n<td>closeable</td>\n<td>&#x63A7;&#x5236;&#x5BF9;&#x8BDD;&#x6846;&#x5173;&#x95ED;&#x7684;&#x65B9;&#x5F0F;&#xFF0C;&#x503C;&#x53EF;&#x4EE5;&#x4E3A;&#x5B57;&#x7B26;&#x4E32;&#x6216;&#x8005;&#x5E03;&#x5C14;&#x503C;&#xFF0C;&#x5176;&#x4E2D;&#x5B57;&#x7B26;&#x4E32;&#x662F;&#x7531;&#x4EE5;&#x4E0B;&#x503C;&#x7EC4;&#x6210;&#xFF1A;<br><strong>mask</strong> &#x8868;&#x793A;&#x70B9;&#x51FB;&#x906E;&#x7F69;&#x533A;&#x57DF;&#x53EF;&#x4EE5;&#x5173;&#x95ED;&#x5BF9;&#x8BDD;&#x6846;<br><strong>esc</strong> &#x8868;&#x793A;&#x6309;&#x4E0B; esc &#x952E;&#x53EF;&#x4EE5;&#x5173;&#x95ED;&#x5BF9;&#x8BDD;&#x6846;<br>&#x5982; &apos;mask&apos; &#x6216; &apos;esc,mask&apos;<br>&#x5982;&#x679C;&#x8BBE;&#x7F6E;&#x4E3A; true&#xFF0C;&#x5219;&#x4EE5;&#x4E0A;&#x5173;&#x95ED;&#x65B9;&#x5F0F;&#x5168;&#x90E8;&#x751F;&#x6548;<br>&#x5982;&#x679C;&#x8BBE;&#x7F6E;&#x4E3A; false&#xFF0C;&#x5219;&#x4EE5;&#x4E0A;&#x5173;&#x95ED;&#x65B9;&#x5F0F;&#x5168;&#x90E8;&#x5931;&#x6548;</td>\n<td>String/Boolean</td>\n<td>true</td>\n</tr>\n<tr>\n<td>placement</td>\n<td>&#x4F4D;&#x4E8E;&#x9875;&#x9762;&#x7684;&#x4F4D;&#x7F6E;<br><br><strong>&#x53EF;&#x9009;&#x503C;</strong>:<br>&apos;top&apos;, &apos;right&apos;, &apos;bottom&apos;, &apos;left&apos;</td>\n<td>Enum</td>\n<td>&apos;right&apos;</td>\n</tr>\n<tr>\n<td>onVisibleChange</td>\n<td>&#x5F39;&#x5C42;&#x663E;&#x793A;&#x6216;&#x9690;&#x85CF;&#x65F6;&#x89E6;&#x53D1;&#x7684;&#x56DE;&#x8C03;<br><br><strong>&#x7B7E;&#x540D;</strong>:<br>Function(visible: Boolean, type: String) =&gt; void<br><strong>&#x53C2;&#x6570;</strong>:<br><em>visible</em>: {Boolean} &#x5F39;&#x5C42;&#x662F;&#x5426;&#x663E;&#x793A;<br><em>type</em>: {String} &#x89E6;&#x53D1;&#x5F39;&#x5C42;&#x663E;&#x793A;&#x6216;&#x9690;&#x85CF;&#x7684;&#x6765;&#x6E90; fromContent &#x8868;&#x793A;&#x7531;Dropdown&#x5185;&#x5BB9;&#x89E6;&#x53D1;&#xFF1B; fromTrigger &#x8868;&#x793A;&#x7531;trigger&#x7684;&#x70B9;&#x51FB;&#x89E6;&#x53D1;&#xFF1B; docClick &#x8868;&#x793A;&#x7531;document&#x7684;&#x70B9;&#x51FB;&#x89E6;&#x53D1;</td>\n<td>Function</td>\n<td>-</td>\n</tr>\n<tr>\n<td>animation</td>\n<td>&#x663E;&#x793A;&#x9690;&#x85CF;&#x65F6;&#x52A8;&#x753B;&#x7684;&#x64AD;&#x653E;&#x65B9;&#x5F0F;</td>\n<td>Object/Boolean</td>\n<td>-</td>\n</tr>\n</tbody>\n</table>\n<h2 id=\"aria-and-keyboard\">ARIA and Keyboard<a href=\"#aria-and-keyboard\" class=\"anchor\">#</a></h2><table>\n<thead>\n<tr>\n<th style=\"text-align:left\">&#x952E;&#x76D8;</th>\n<th style=\"text-align:left\">&#x8BF4;&#x660E;</th>\n</tr>\n</thead>\n<tbody>\n<tr>\n<td style=\"text-align:left\">esc</td>\n<td style=\"text-align:left\">&#x6309;&#x4E0B;ESC&#x952E;&#x5C06;&#x4F1A;&#x5173;&#x95ED;dialog&#x800C;&#x4E0D;&#x89E6;&#x53D1;&#x4EFB;&#x4F55;&#x7684;&#x52A8;&#x4F5C;</td>\n</tr>\n<tr>\n<td style=\"text-align:left\">tab</td>\n<td style=\"text-align:left\">&#x6B63;&#x5411;&#x805A;&#x7126;&#x5230;&#x4EFB;&#x4F55;&#x53EF;&#x4EE5;&#x88AB;&#x805A;&#x7126;&#x7684;&#x5143;&#x7D20;&#xFF0C; &#x5728;Dialog&#x663E;&#x793A;&#x7684;&#x65F6;&#x5019;&#xFF0C;&#x7126;&#x70B9;&#x59CB;&#x7EC8;&#x4FDD;&#x6301;&#x5728;&#x6846;&#x4F53;&#x5185;</td>\n</tr>\n<tr>\n<td style=\"text-align:left\">shift+tab</td>\n<td style=\"text-align:left\">&#x53CD;&#x5411;&#x805A;&#x7126;&#x5230;&#x4EFB;&#x4F55;&#x53EF;&#x4EE5;&#x88AB;&#x805A;&#x7126;&#x7684;&#x5143;&#x7D20;&#xFF0C;&#x5728;Dialog&#x663E;&#x793A;&#x7684;&#x65F6;&#x5019;&#xFF0C;&#x7126;&#x70B9;&#x59CB;&#x7EC8;&#x4FDD;&#x6301;&#x5728;&#x6846;&#x4F53;&#x5185;</td>\n</tr>\n</tbody>\n</table>\n"}