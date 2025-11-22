



% preamble chirp


fs = 48e3;


pw = 100e-3;


dt = 1/fs;


bw = 12e3;

t = [dt:dt:pw];

t = t - pw/2;

slope = bw/pw;

lfm = exp( 1i *pi* slope *t.^2 );

