M = 'Hello world'; 
% Now encode:
Mbinlong = reshape(dec2bin(double(M),7).',[],1)
sound(real(double(Mbinlong)))
% Now decode:
mess = char(bin2dec(reshape(Mbinlong,7,[]).').')

% send white noise and cross correlate what we received and what we sent
% leave pulse shaping for later
% convert to 1s and -1s
% turn those 1s and -1s into a bunch of pulses
% pulse shaping and carrier synchronization are doing 2 different things
% carrier synchronization handles shift between 2 computers
% don't use pulse shaping yet just use rectangular pulse for now
% bin_str = 2* bin_str - 1
% bin_str_us = upsample(bin_str, 20)
% pulse = ones(20, 1)
% X_I = conv(bin_str_us, pulse)
% X = X_I * cos(2pifct) then play this on the computer with sound
% take X_I and multiply it by cos
% on the receiver multiply by cos and LPF
% y_c = y*cos(2pifct..)
% y_s = y*sin(2pifct..)*j
% y_b = y_c + y_s