```
public class Main {
    public static void main(String[] args) {
        int current_account = 100;
        int payment = 1001; // <- тут вносится значение платежа внесенного клиентом
        int payment_bonus;
        if (payment>=1000) {
            payment_bonus = payment/100;
            current_account = current_account + payment + payment_bonus;
            System.out.println("Cумма на счету клиента: " + current_account + " рублей");
            System.out.println("Бонус составил: " + payment_bonus + " рублей");
            }
        else {
            current_account = current_account + payment;
            System.out.println("Cумма на счету клиента: " + current_account + " рублей");
            System.out.println("Бонус составил: 0 рублей");
            }
    }
}
```