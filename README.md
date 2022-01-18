Hacky little script based on [https://gist.github.com/michaellihs/d2070d7a6d3bb65be18c](https://gist.github.com/michaellihs/d2070d7a6d3bb65be18c) 
which will accept inbound ssh connections with any username/password combination and rickroll them (see below).

**This script is intended as a joke and is not designed to be secure. Run it only at your own risk. It is never a good idea to open up your computer to external threats, and this SSH server, while intended to provide no commands to users, should not be seen as foolproof/safe to run without putting your server at risk.**

```bash
ttftffftttttttttffffffLftfftttttttttt111tttt1111111tttt11t111tttt111111tttttttttttttttttttt11111111t
ttfttttttttttttttfffLLLftfffffffffttttt1111t11111ttffffftttt1111111111111111tttttfftttttttt1111111tt
ttftttttttttttttffffLffttffffffffLLfttttttfttt11ttt1iiii;i11tttt111111tttttffffftffffttttttt111111tt
ttttttttttttttttfffLLttffffffLLffffttttttttttt1tt1::,,,,,,:;1ttt111111tfftfffffftttfffffttt1111t1tt1
ttttttttttttffffttffftffffffffffttfftttttt1ttt11i;:,,,,,,,,,:1111t1111111tffffLLffttfLfftt11111ttttt
ttttttttttffLLLLfttttffLLLfftttttfLftttttttffft1;:::;;;;;;;::it11t111tt111tttffffftttfttttt1111ttttt
ttttttttffLLLLLLLffttfLLLfttfffftfLLtttttfffffti:;;ii111111i:itt11111tft11111ttffffttt1ttffftt1ttttt
tttttttfffLLLLLLLLLftffftttffLffftffttttfffffft;:;;;;;iiiiii;ittt1111ttt1tttt11tffLfttttfffffftttttt
tttttttffLLLLLLLLLfttttffftffLLftfftttttffffffti;;;;;;;ii;iiitttt11111111ttftttttttt1ttffffffffffttt
tttfftfffLLLLLLLLLftffftfLftffffLLLftttttfffff1iii;;i;;i1i1i1tttt11111ttt1ttt1tfttt111tfffffLLfLfttt
ttfLffffffLLLLLLLffffLLfffffLfffLLLftttttttfft1i;;;;;;;iiiiitfft111111ffft11t11tt1tttttffffLLLLLffft
tffftfttttfLLLffttttffffftfLLLLfLLLftttftt1111111i;;;;iiii111t111t1111tffttfftt11tfft1tffLLLLLLLLfff
ttffftttttffLftttttttttttttfLLLffLLftttt1tttt11tti;;;iiiii111111111111tffttffftttttttt1ttfLLLfffffff
ttfLffffffftttfffffffffttfttfLLfffLftttttffft1111i;;;;;ii111tfttt11111ttt1tffttt11ttttttttfLfftfttft
ttffffffffftttfffffffffttffftffffftttttfffft11t11i;;;;iii1i:;1ttft11111111ffttfftttfffffLfttttfffffL
ttffffffffttttffffffffttttttttttffftttttft111tttiii;;iiii1;,,,:;i1111111111t1tfft1ttffffLLftttfLLLLL
tttffffffffttffffffffttttttttttfffftttt1111i;:;iiii;;;i;11:,,.....,:;i1tft1111tt111tffffLfftttffLLLf
ttttttttfffttfffttttttttfftt111tfffttt11i;,,..:i;;;i;ii1t1,,..........,:i1111ttt1111tffffffftffLLLLf
tfttttttttttttttttttttffffttttt1tffti;:,,.....,;;;iiii1ti,,,.............;1111ttttt11111ttfftffffftt
tttttffffttttttfffftttffffttffttttf1:.........,;:;;;;;;;,.,,,............:1tt1ttffff11ttttt1ttttttft
tttttffffftttffftfft1ttffftfffttttf1,..........,;;;;;;;:.:ii;;:,.........:tttt1tfffttttffft111tfffff
1tttffffftt1ttfffftt11tffttfttttt1t1,...........ii;;;::,,;i;;ii:.........:tttt1tfft11tfffffft1fLLfLf
tftttffttttt11tftt1tttt1ttttttttt11i,..........,1i;;::,.:i;;;;i:.........,1t1t11ttttttttfftt111fffLf
tfftttttttffttt11tttffttt1tttffft11i,..........,ii;:::,.,:;;iii:..........it111111tfft1ttt11tt1tffft
ttttttttttttttt11tttttttt1tfffffftti,...........:::::,....:;;ii:..........:tt111ttfffftttttffftttttt
tfffttttfffffft11ttttttttttfffffft1i,...........:::::,.....,:;;:.... ......,1t111ttttffttttttttffttf
tfffttttfffffft11tftttffttttfffft111:...........:::::,........,..,..........,1111tffffffttfffffffttf
tfffttttfffffft1tttttttftttttttttt11:...........::,:,........ ...:;,.........:111tffffLfttfffttffttf
tffftttttttfft11ttttttttttffttttttti,...........:::,,.............,...........,i1tffffLfttfffttffttf
tttttttttttttt111tttttttttffftttfft;,:;:........:::,.............. ...........:11tfffffftttffttffttt
tttttttttttttt11ttttttttttfftttttftii1i;:.......:::,.......... ..............:t111tttttt11tttttffttt
ttttt1tttttttt11tfttttfftttttffttt1ii;ii;,......::,,........................:1111ttttttt11ttttttfttt
1tttt1ttfttttt11tfffffffttttfffft11i;;ii;,......:,,,..........:........   .;t1111ttttttt111tttttft1t
1tttt1tttttttt11tttttttttttttttttt11;:;i:,,.....:,.................. .;i;;1tt1111tttt1t1111ttttttt1t
111111tttttttt111t111ttttttttttttt11i:,,:1;....,::....................:1ttttt11111111111111111111111
111111111tt1111111111tttttttttttttt11i;;1t:....:::::...................;tttttttt11111111111111111111
1111111111111111111111ttttttttttttt111ttt1,,,.,:::::,..................,1ttttttt11111111111111111111
111111111111111111111111tttttttttt1111111i,::.,;::;:,...................;ttttttttt111111111111111111
1111111111111111111111111ttttttt11111111t;.,,.,;;;;;,...................,1ttttttt11t1111111tttt11111
111111111111111111111111111111111111111t1:..,,:;;;;;:,...................;ttttttt111t11111ttttt11111
111111111111111111111111111111111111111ti,,,::;;;;;;;:,..................,1tttttttt1tttt11tttttt1111
111111111111111111111111111111111111111t;,,::,;;;ii;;::,..................it1tttttttttttttttttt11111
```