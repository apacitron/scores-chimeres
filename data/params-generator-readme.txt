//////////////////// [ text define -k $0-PARAMS ] ///////////////////////////
///////// descritpion des valeurs de table par fonction /////////////////////
/////////////////////////////////////////////////////////////////////////////
//
//
//// cf. [pd GENERATEUR-PARAMS] :

/////////////// MOTIF PHASOR
P0 	:	freq1 phasor1
P1 	:	freq2
P2 	:	freq3
/////////////// STRUCTURE
P3	:	duree motif (ms)
P4	: 	durée morceau (mn)
P5	:	nb total de repetition du motif ds le morceau P4 / P3
P6	:	nb de mouvement dans le morceau (rdm 3 + 1)
P7	: 	nb de repetition du motif par mouvement 

/////////////// LFOS
P8 9 10		:	rdm direction (shape) LFO 1 2 3 (1 / -1)
P11 12 13 	: 	freq LFO1 LFO2 LFO3
/////////////// MOODULO LENGTH DISTRIB ROUTING
P14	:	rdm modulo seq length (3~12)
///////////////
P15 - P20	: FREE-params
/////////////// PROBA P16 - P23 rdm 0~1
P16	:	valeurs step1 de $0-proba (rdm 0~1)seuil LFO2
P17	:	valeurs	step2 ''
P18	:	valeurs	step3
P19	: 	valeurs	step4
P20	:	valeurs	step5
P21	:	valeurs	step6
P22	:	valeurs	step7
P23	:	valeurs	step8
//
P24 -25 : FREE
/////////////// MULTI 26 - 33
P26	:	valeurs step1 de $0-multi (rdm 1~15)* LFO3
P27	:	valeurs	step2 ''
P28	:	valeurs	step3
P29	: 	valeurs	step4
P30	:	valeurs	step5
P31	:	valeurs	step6
P32	:	valeurs	step7
P33	:	valeurs	step8
/////////////// FREE
P34 - 40 FREE
/////////////// ROUTING 41
P41 :	numero de depart ligne routing, puis +1 % nb de mouvements / 4

