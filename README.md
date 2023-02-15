# ChallengeB

# challenge b
#first sound to stop at the top
live_loop :fg do
  16.times do
    sample :drum_cymbal_closed
    sleep 0.5
  end
  stop
end

live_loop :dsa do
  16.times do
    sample :drum_heavy_kick, amp: 2
    sleep 1
  end
  stop
end

live_loop :s do
  12.times do
    sample :drum_snare_soft
    sleep 2
  end
  stop
end

#live_loop :sk do
4.times do
  sample :drum_splash_hard, sustain: 3
  sleep 2
end
stop
end

#live_loop :sk do
8.times do
  sample :drum_cymbal_hard
  sleep 0.5
end
stop
end
