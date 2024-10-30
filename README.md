# Likhtman-McLeish Model (LM Model)  
ref: Likhtman, A. E.; McLeish, T. C. B. "Quantitative Theory for Linear Dynamics of Linear Entangled Polymers". *Macromolecules* __2002__, 35, 6332-6343. 

$$
G(t)= G_e \left[\frac{4}{5} \mu(t) R(t) + \\
\frac{1}{Z} \sum^N_{p=Z}\exp \left( -\frac{2p^2t}{\tau _ R}\right) + \\
\frac{1}{5Z}\sum^{Z-1}_{p=1}\left(-\frac{p^2t}{\tau_R}\right) \\
\right]
$$

$$\begin{align}
G'(\omega) &= \omega \int_0^\infty G(t) \sin \omega t \ dt \\
G''(\omega) &= \omega \int_0^\infty G(t) \cos \omega t \ dt \\
G^*(\omega) &= G'(\omega) + iG''(\omega)\\
&=i\omega \int_0^\infty G(t) e^{-i\omega t} \ dt \\
e^{i\omega t} &= \cos \omega t + i \sin \omega t \\
e^{-i\omega t} &= \cos \omega t - i \sin \omega t
\end{align}
$$

The first term is the contributions due to escape from the tube described by $\mu(t)$ and $R(t)$.  
The second term is longitudinal modes relaxation.  
The third term is fast Rouse motion inside the tube.  
$\mu(t)$: the tube-segment occupation function;  
$R(t)$: the constraint release relaxation function;  

$$R(t,v_{\nu}) = 1 - \frac{C_R}{Z}\left( \frac{c_{\nu}t}{\tau_e} \right)^{1/4} , C_R \approx  1.8$$

$$\begin{align}
\mu(t) &= \frac{8\tilde{G} _f}{\pi ^2} \sum _{p=1,odd} ^{p ^*} \frac{1}{p ^2} \exp \left( - \frac{tp ^2}{\tau _{df}} \right) &+ 
\int _{\epsilon ^\*} ^{\infty} \frac{0.306}{Z\tau _e ^{1/4}\epsilon ^{5/4}} \exp (-\epsilon t) d \epsilon \\
&= ... &+ \int _{\ln \epsilon ^\*} ^{\infty} \frac{0.306}{Z(\tau _e\epsilon) ^{1/4}} \exp (- \epsilon t) d \ln \epsilon
\end{align}$$

Here:  

$$
\epsilon ^\* = \frac{1}{\tau _e Z^4} \left(\frac{4\times 0.316}{1 - 8 \tilde{G} _f / \pi^2 \sum _{p=1,odd} ^{p ^\*}\frac{1}{p ^2}}\right) ^4 ,  p ^\* \sim  \sqrt{Z/10}
$$

$$
\tau_{df}(Z)/\tau_d^{(0)}(Z) = 1- \frac{2C_1}{Z^{1/2}} + \frac{C_2}{Z} + \frac{C_3}{Z^{3/2}}
$$
$$
\tilde G_f(Z) = 1 - \frac{C_1}{Z^{1/2}} + \frac{C_4}{Z} + \frac{C_5}{Z^{3/2}}
$$
By fitting simulation data for Z = 2 ~ 100 gives:
$$
C_1 = 1.69; C_2 = 4.17; C_3 = -1.55; C_4 = 2.0; C_5 = -1.24
$$

$\tau_d^{(0)}$ is the reptation or disentanglement time, and $\tau_d^{(0)} = 3Z^3\tau_e$
