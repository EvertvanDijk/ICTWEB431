```mermaid
flowchart TD
    Order([Place Order]) --> ship[Verify order]
    ship --> address{"Verify Address?"}
    address -- Yes --> pick[Pick & Pack]
    address -- No --> informcustomer[Notify Customer]
    informcustomer  --> update[update address ]
    update --> address
    pick --> shipped[Ship Order]
    shipped --> delivered([Delivered])
```


