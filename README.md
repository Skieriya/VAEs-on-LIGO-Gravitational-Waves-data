# VAEs-on-LIGO-Gravitational-Waves-data

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1w0DKJEy7RmOIiQsvr0loQe8gU7bszH8Y#scrollTo=dayKgVoEh1KJ)

Okay so i trained a VAE here on the synthetic gravitational wave data generated using

and why gravitational waves??? cause mostly the data which comes to us is noisy and we have to clean it to understand it so how about something which can be trained on noisy data and here you go VAEs YAYYY.

signal(t) = exp(-t * spin) * cos(mass * 10 * t) + noise

My intuition behind choosing VAEs is that i recently studied VAEs and learned about thier latent space representation capabilities and found out that current approaches doesnt use latent represenation because it uses clean fixed signals.
So i thought VAEs can help here and made then made this.

# Evaluation 

<img width="1089" height="590" alt="image" src="https://github.com/user-attachments/assets/4b506b26-5092-4496-aace-845c0fcc1cb5" />

I used MAPE ( Mean absolute percentage error ) here because it penalize it heavily for missing both small and large values

