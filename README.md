```
public class Main {
    public static void main(String[] args) {
        int currentAccount = 100;
        int payment = 1111; // <- тут вносится значение платежа внесенного клиентом
        int paymentBonus;
        if (payment >= 1000) {
            paymentBonus = payment / 100;
            currentAccount = currentAccount + payment + paymentBonus;
            System.out.println("Cумма на счету клиента: " + currentAccount + " рублей");
            System.out.println("Бонус составил: " + paymentBonus + " рублей");
        } else {
            currentAccount = currentAccount + payment;
            System.out.println("Cумма на счету клиента: " + currentAccount + " рублей");
            System.out.println("Бонус составил: 0 рублей");
        }
    }
}
```