# Prosta sieć rekurencyjna (RNN)
Sieć RNN zaprojektowana jest do przetwarzania danych sekwencyjnych i może być stosowana do problemów takich jak analiza tekstów, dźwięków czy szeregów czasowych. W notatniku zaimplementowano prostą sieć przeznaczoną do tłumaczenia maszynowego, umożliwiając przekład tekstów z jednego języka na drugi.

Uproszczony opis architektury:
 - **Wejście do sieci (x)**: Każdy element sekwencji (np. słowo w zdaniu) jest podawany do sieci jako wektor w kolejnych krokach czasowych.
 - **Pierwsza warstwa ukryta**: Sieć ma początkowy stan ukryty h0h_0h0, który zazwyczaj jest wektorem zerowym. Wejście x jest przetwarzane razem z h przez funkcję aktywacji, tworząc nowy stan ukryty hn.
 - **Przepływ informacji przez czas**: W każdym kroku czasowym t, nowy stan ukryty h jest obliczany na podstawie poprzedniego stanu oraz bieżącego wejścia za pomocą wag W.
 - **Generowanie wyjścia yt w każdym kroku**: Każdy stan ukryty ht jest przekształcany przez warstwę wyjściową z wagami Wy, generując odpowiedź yt.
 - **Przetwarzanie sekwencji**: Proces powtarza się dla kolejnych kroków t=1,2,3,...,n, aż cała sekwencja zostanie przetworzona.

![image](https://github.com/user-attachments/assets/739ec2f5-da19-4a0b-a047-3629c4e86028)
