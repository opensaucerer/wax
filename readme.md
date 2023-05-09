# wax

an iot enabled decentralized electric meter powered by solana

## Why Wax?

I've always been fascinated about the idea and then came my student IT period. To ensure I ace my presentation, I decided to make a project and felt `wax` would be the right one to work on since I state in my student logbook that my IT was centered around IoT.

## What Wax?

The working is simple. Wax subsribes to the Solana blockchain and listens for changes on a particular account. In a real setting, this wallet address is what you can refer to as the meter number. When there wallet balance changes, `wax` checks to see if the balance meets a required threshold and depending on the threshold, it sends a signal via mqtt to the microcontroller which then powers on a particular led light.

- Red: Zero balance
- Yellow: Low balance
- Green: High balance

## When Wax?

The current implementation is just a proof of concept and can be built upon to become better. Essentially, a meter provides a different switch interface whereby light is allowed to travel depending on balance threshold and that's what `wax` does or can be made to become.
