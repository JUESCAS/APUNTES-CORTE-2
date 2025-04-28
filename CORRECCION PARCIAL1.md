# Corrección del parcial 
$$ \ F(s) = \frac{6s}{(s - \frac{5}{2})(s^2 + 4s + 8)}\$$
$$ \ F(s) = \frac{A}{s - \frac{5}{2}} + \frac{Bs + C}{s^2 + 4s + 8}\$$
$$ \ A = \left[ \frac{6s}{(s - \frac{5}{2})(s^2 + 4s + 8)} \cdot \left( s - \frac{5}{2} \right) \right] \Bigg|_{s = \frac{5}{2}}\$$
$$ \ A = \frac{6 \left( \frac{5}{2} \right)}{\left( \frac{5}{2} \right)^2 - 4 \left( \frac{5}{2} \right) + 8}\$$
$$ \ A = \frac{60}{17}\ $$

$$ \ Bs + C = \left[ \frac{6s}{(s - \frac{5}{2})(s^2 + 4s + 8)} \cdot (s^2 + 4s + 8) \right] \Bigg|_{s = -2 + 2i}\$$
$$\ Bs + C = \frac{6(-2 + 2i)}{-2 + 2i - \frac{5}{2}}\$$
$$\ -2B + 2Bi + C = \frac{312}{97} - \frac{120}{97}i\$$
$$\ -2Bi = -\frac{120}{97}i \$$
$$\ B = \frac{60}{97}\$$
$$\ C = \frac{312}{97} + 2 \left( \frac{60}{97} \right)\$$
$$\ C = \frac{432}{97}\$$
$$\ F(s) = \frac{\frac{60}{17}}{s - \frac{5}{2}} + \frac{\frac{60}{97}s + \frac{432}{97}}{s^2 + 4s + 8}\$$
$$\ f(t) = \mathcal{L}^{-1} \left[ \frac{\frac{60}{17}}{s - \frac{5}{2}} + \frac{\frac{60}{97}s + \frac{432}{97}}{(s + 2)^2 + 4} \right]\$$
$$\ f(t) = \frac{60}{97} e^{-2t} \cos(2t) + \frac{432}{97} e^{-2t} \sin(2t) \$$

$$\ 2\ddot{x} + 2\dot{x} + x = 1, \quad \dot{x}(0) = 2, \quad x(0) = 0\ $$
$$\ s^2 X(s) - s x(0) - \dot{x}(0) + 2(s X(s) - x(0)) + X(s) = \frac{1}{s}\ $$
$$\ 2s^2 X(s) - 4 + 2s X(s) + X(s) = \frac{1}{s}\ $$
$$\ 2s^2 X(s) - 4 + 2s X(s) + X(s) = \frac{1}{s} + 4\ $$
$$\ X(s)(2s^2 + 2s + 1) - 4 = \frac{1}{s}\ $$
$$\ X(s) = \frac{1 + 4s}{s(2s^2 + 2s + 1)}\$$
$$ C = \frac{2s - 3}{(s - 1)(s^2 + 6s + 10)(s^2 + 8s + 17)}$$

$$ C = \frac{d}{ds} \Bigg|_{s = -2} \left[ \frac{2s - 3}{s^5 + 13s^4 + 61s^3 + 107s^2 + 120s - 170} \right]$$

$$ C = \frac{d}{ds} \Bigg|_{s = -2} \left[ \frac{2s - 3}{s^5 + 13s^4 + 61s^3 + 107s^2 + 120s - 170} \right] = \frac{(2s - 3)(5s^4 + 52s^3 - 138s^2 - 214s + 120) - 2(s^5 + 13s^4 + 61s^3 - 107s^2 + 120s + 170)}{(s^5 + 13s^4 + 61s^3 + 107s^2 + 120s - 170)^2}$$

$$ C = \frac{(2s - 3)(5s^4 + 52s^3 - 138s^2 - 214s + 120) - 2(s^5 + 13s^4 + 61s^3 - 107s^2 + 120s + 170)}{(s^5 + 13s^4 + 61s^3 + 107s^2 + 120s - 170)^2}$$

$$ C = \frac{114s^5 - 447s^4 - 14s^3 + 642s^2 + 240s + 360 - 2s^5 - 26s^4 - 122s^3 + 214s^2 - 240s - 340}{s^{10} + 169s^8 + 3721s^6 - 11449s^4 + 14400s^2 + 28900}$$

$$ C = \frac{112s^5 - 473s^4 - 136s^3 + 856s^2 + 20}{s^{10} + 169s^8 + 3721s^6 - 11449s^4 + 14400s^2 + 28900} $$

$$ C = \frac{112(-2)^5 - 473(-2)^4 - 136(-2)^3 + 856(-2)^2 + 20}{(-2)^{10} + 169(-2)^8 + 3721(-2)^6 - 11449(-2)^4 + 14400(-2)^2 + 28900}$$

$$ C = \frac{-6620}{185748}$$

$$Ds + E = \frac{s + 5}{(s - 1)(s + 2)^2 (s^2 + 6s + 10)(s^2 + 8s + 17)} (s^2 + 6s + 10)$$
$$D(-3 + i) + E = \frac{2(-3 + i) - 3}{((-3 + i) - 1)((-3 + i) + 2)^2 ((-3 + i)^2 + 8(-3 + i) + 17)} $$
$$ -3D + Di + E = \frac{15}{34} + \frac{8}{34}i $$
$$ Di = \frac{8}{34}i $$
$$ D = \frac{8}{34} $$
$$ E = 3D + \frac{15}{34} $$
$$ E = 3 \left( \frac{15}{34} \right) $$
$$ E = \frac{45}{34} $$
$$ Fs + G = \frac{2s - 3}{(s - 1)(s + 2)^2 (s^2 + 6s + 10)(s^2 + 8s + 17)} (s^2 + 8s + 17) $$
$$ F(-4 + i) + G = \frac{2(-4 + i) - 3}{((-4 + i) - 1)((-4 + i) + 2)^2 ((-4 + i)^2 + 6(-4 + i) + 10)} $$
$$ -4F + Fi + G = \frac{-52}{425} + \frac{89}{425}i $$
$$ -Fi = \frac{89}{425}i $$
$$ F = \frac{-89}{425} $$
$$ G = -4 \left( \frac{89}{425} \right) + \frac{52}{425} $$
$$ G = \frac{-304}{425} $$
$$ F(s) = \frac{-1}{3978} \cdot \frac{1}{s - 1} + \frac{7}{30} \cdot \frac{1}{(s + 2)^2} - \frac{6620}{185748} \cdot \frac{1}{s + 2} + \frac{8}{34} \cdot \frac{s + 45}{34} \cdot \frac{1}{(s + 3)^2 + 9} + \frac{-89}{425} \cdot \frac{s - 304}{425} \cdot \frac{1}{(s + 4)^2 + 1} $$
$$ \mathcal{L}^{-1} \left[ \frac{-1}{3978} \cdot \frac{1}{s - 1} + \frac{7}{30} \cdot \frac{1}{(s + 2)^2} - \frac{6620}{185748} \cdot \frac{1}{s + 2} + \frac{8}{34} \cdot \frac{s + 45}{34} \cdot \frac{1}{(s + 3)^2 + 9} + \frac{-89}{425} \cdot \frac{s - 304}{425} \cdot \frac{1}{(s + 4)^2 + 1} \right] $$
$$ f(t) = - \frac{e^{-t}}{3978} + \frac{7t e^{-2t}}{30} - \frac{6620 e^{-2t}}{185748} + \frac{1}{34} \left( 8 e^{-3t} \cos(3t) + 7 e^{-3t} \sin(3t) \right) + \frac{1}{425} \left( 89 e^{-4t} \cos(t) - 304 \cdot 7 e^{-4t} \sin(t) \right) $$



