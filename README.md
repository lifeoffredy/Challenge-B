# Challenge-

#snare two times
sample :drum_snare_soft
sleep 2
sample :drum_snare_soft
sleep 2

#kick four times
sample :drum_heavy_kick, amp: 2
sleep 1
sample :drum_heavy_kick, amp: 2
sleep 1
sample :drum_heavy_kick, amp: 2
sleep 1
sample :drum_heavy_kick, amp: 2
sleep 1

#cymbal eight times
sample :drum_cymbal_closed
sleep 0.5
sample :drum_cymbal_closed
sleep 0.5
sample :drum_cymbal_closed
sleep 0.5
sample :drum_cymbal_closed
sleep 0.5
sample :drum_cymbal_closed
sleep 0.5
sample :drum_cymbal_closed
sleep 0.5
sample :drum_cymbal_closed
sleep 0.5
sample :drum_cymbal_closed
sleep 0.5

#ALL TOGETHER NOW
sample :drum_splash_hard, sustain: 3
sample :drum_cymbal_hard
sample :drum_cowbell, amp: 1.5
#But also play the snare, kick, and cymbal together
live_loop :soft do
  sample :drum_snare_soft
  sleep 2
end

live_loop :heavy do
  sample :drum_heavy_kick, amp: 2
  sleep 1
end

live_loop :closed do
  sample :drum_cymbal_closed
  sleep 0.5
end
