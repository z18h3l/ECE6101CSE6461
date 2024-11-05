java c
ECE6101/CSE6461 
Homework 3 Assignment 
Autumn 2024
Expected Completion Date: November 12, 2024
Solve problems 4-1, 4-2, 4-7, 4-8, 4-9, 4-10, 4-11, 4-12, 4-15, 4-17, 4-18 in the Schwartz book.
[4-1]  Derive the expression below for the average transmission time for a frame. in the go-back-N protocol:
where TI  is the time required to transmit a frame, p is the probability of a frame. error, tT  = tI  + tout  is the minimum time between successive frames, and a ≡ tI/tT.
[4-2]  The normalized data throughput rate D/C expression for the go-back-N protocol as a function of packet length l, control bit length of l′ , and link capacity C is as follows:

Plot D/C as a function of packet length l for the following two cases:
1.  l′ = 48bits, the length is 1500km, the propagation speed over the link is 150,000km/s, processing delay is 30ms, pb   =  10 − 5,  C=1200pbs.   Bit  errors  are independently dis- tributed.  Take tout  = 2tp + 2tI, as in the book, with processing time included in the propagation delay.
2.  Same as in case 1, except that C=9600bps
[4-7]  Plot the normalized data throughput rate D/C given in Question [4-2], as afunction of packet length lfor the following three examples with pb  = 10−5 , l′ = 48bits and l varying between 10 and 10,000 bits (plot x axis in log scale):
1.  Terrestrial Link 1: 2tp = 100ms, C = 4, 800bps
2.  Terrestrial Link 2: 2tp = 100ms, C = 48, 000bps
3.  Satellite Link: 2tp  = 700ms, C = 48, 000bps
[4-8]  Taking (a − 1)p ≪ 1 in the Equation given in [4-2], show that the optimum packet length is given by

[4-9] Find the optimum packet length l and the corresponding data rate D in bps for the following cases:
1.  l′ = 48bits, propagation speed on the link is 150,000 km/s, link length is 300km, there is negligible processing delay, pb  = 10−5 , C = 1200bps.
2.  Same as the first case, but C = 9600bps.
3.  Satellite link, l′ = 48bits, tp  = 0.25s, pb  = 10−5 , C = 56kbps
4.  Same as the third case, but pb  = 10−7
[4-10] Following is a simplified infinite-sequence-number model of the HDLC protocol analyzed in the textbook.  An RR control frame. is used to acknowledge correct receipt of an I-frame. of length tIAn REJ frame. is used to reject a frame. received in error, on the first transmission of that frame. only. Subsequent retransmissions of the frame, if received in error, are ignored; a timeout of tout  is then used to control retransmission.  Both the RR and the REJ frames are received代 写ECE6101/CSE6461 Computer Communication Networks Homework 3 Assignment Autumn 2024Statistics
代做程序编程语言 at the transmitter at time tack  after the transmission of an I-frame.  Take tout  ≥ tack. Find an expression for the maximum frame. transmission time λmax.  Make any assumptions required on the length of tout  and tack to simplify the analysis.  (For example, tout  is a multiple of tI)
[4-11]  Refer to the problem [4-2].  Calculate and plot D/C vs.  l for the two examples given there, using the results of the HDLC analysis:
where T1 represents the random time required to transmit the first repeat, E[T1] is its average value, and T2  is the average time required for transmission on subsequent retransmissions. Take M = 8 as the maximum sequence number.  Compare with the results of problem  [4-2]. Assume that bit errors are independent.
[4-12]  Consider the terrestrial error-probability model discussed in the textbook.  Show that the optimim packet length for this model is given by

[4-15] A suggestion is made that the RR frame. in HDLC be used not only for positive acks, but for negative acks as well.  After all, it is argued, both the RR and REJ (NACK) frames positively acknowledge receipt of frame. N(R)-1 and all frames preceding and indicate that frame. N(r) is expected.  They are thus implicitly carrying out the same function.  Hence, why not use RR in all cases. Explain why this could not be possible.
[4-17] It is noted in the text that no more than M-1 unacked frames can be outstanding at any one time if M is the maximum sequence number.  Explain why this is a necessary condition for the protocol always to work correctly. A counter-example, showing what might happen if M unacked frames were outstanding, would be helpful.  Hint:   Consider the following possible scenario.  Station A transmit I-frames 0,  1, 2, ..., M-1, and then stops.  Station B, silent to this point, now transmits an I-frame.  How does this differ from the case in which A is always silent?
[4-18]  Explain by an example,  with one node serving as transmitter and the other  as receiver, why the selective repeat scheme requires a reordering buffer at the receiver.  Show a series of sequentially numbered frames being transmitted.  A copy of each frame. is stored at the transmitter until acked positively.  A number of the frames are hit by errors.  Indicate with diagramshow error recovery is carried out. Sketch a block diagram of transmitter and receiver incorporating a  “waiting for ack” buffer at the transmitter and a reordering buffer at the receiver.

         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
