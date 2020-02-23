# eSK8 Proposal

1. **Project overview**

   The objective of this project is to combine the already matured electric skateboard building solution with highly customizable features like programmable different motor output modes and LED light strips, resulting in a powerful and aesthetically pleasing campus commuting vehicle.

2. **Goals and Plans to Meet Them**

   - **Powerful**: The design features hub motors instead of the most commonly used motor-wheel pulley solution, because the latter cannot function as a regular skateboard when powered down. Adopting the former solution gives us more options when using the skateboard. 

   - **Cheap**: Cheap may sound contradictory with powerful, but the top-tier electric skateboards currently on the market can be as costly as $1599 ([Boosted Stealth](https://www.amazon.com/Boosted-BPN-102044-Stealth-Electric-Skateboard/dp/B07D9XKGK6/ref=sr_1_4?crid=3TRR91MPS529Z&dchild=1&keywords=boosted+board&qid=1574561101&sprefix=boosted%2Caps%2C148&sr=8-4)), I will cut off the budget by building as many DIY parts as possible, and buying my parts directly from manufacturers (this can be achieved using AliExpress). Instead of buying a typical electric skateboard RC control which costs 65 dollars, I will build my own using Arduino Micro and NRF24L01 module.

   - **Additional features** 

     - Interchangeable Batteries

       A little door will be cut out from the enclosure case that holds all the batteries, so that when batteries run low in the board, users can instantly get more range by replacing them, and users do not need to charge the entire skateboard when going back to home (Current models on the markets generally does not support interchangeable batteries).

     - Handle

       A 3D printed handle will be added to the side of the board deck for easy lifting and carrying.

     - LED Strip

       LED Strips are located on the two sides of the enclosure case at the bottom of the skateboard, and shine their light on two sides of the skateboard. They are programmed to emit blue light when going forward and red light when applied brakes.

       ![Screen Shot 2019-10-27 at 10.21.25](/Users/ziyuli/Documents/Personal Projects/eSK8/ProposalPhotos/Screen Shot 2019-10-27 at 10.21.25.png)

     - Front Light

       A front light will be added to provide good vision while riding at night, avoiding running into bumps.

     - Motor Modes

       Since the VESC is open-sourced and can be completed modified using corresponding software, I can add two modes: 1. A commuting mode for energy-efficiency driving and 2. Boosted mode for increased acceleration and deceleration.

3. **Current design**

   - CAD![Deck-Proto](/Users/ziyuli/Documents/Personal Projects/eSK8/ProposalPhotos/Deck-Proto.jpg)

   - Schematic Diagram

     ![eSK8](/Users/ziyuli/Documents/Personal Projects/eSK8/ProposalPhotos/eSK8.jpeg)

4. **Contribution to the Robotics Club**

   Since I will be keeping a detailed build log with descriptions and photos, I can leave lots of experience for club members who also want to DIY cool commuting vehicles. The mechanical and electrical engineering skills required by this project are basic but essential to any robot builders, and by implementing these skills, people can get a good train to start. Since the ultimate objective of this project is kind of becoming an "eye-catcher", anyone who wants to re-implement this electric skateboard can get an impressive tool that they can use every day and become a cool guy on campus. Also, unlike ordinary skateboards that have fix appearances and closed source programs, my project will be highly customizable and programmable, so it will serve as a base for anyone who has their own idea and preferences.

5. **Proposed timeline**

   | Time             | Todo                                 | Description                                                  |
   | ---------------- | ------------------------------------ | ------------------------------------------------------------ |
   | January          | Gather parts                         | Some of the parts has to be shipped from China (because it's cheaper that way), which takes a lot of time, so the parts gathering time would be the entire winter vacation. |
   | February-Week1   | Assemble the parts                   | Get the basic electric skateboard functions running.         |
   | February-Week2   | Test additional features             | Hook the lights and LED strips on the control board. 3D print the enclosure case and the handle. |
   | February-Week3-4 | Polish design and real world testing | Further design the skateboard to make it more interactive. Test the overall capability of the skateboard in real world settings. |
   | March-           | Documentation                        | Clear up all the build logs and files I used during build.   |

6. **Budget**

   | Name                           | Purpose                                  | Sample link                                                  | Cost    |
   | ------------------------------ | ---------------------------------------- | ------------------------------------------------------------ | ------- |
   | Hub motor                      | Move the skateboard                      | https://www.aliexpress.com/item/32967381392.html?spm=a2g0o.productlist.0.0.111f3ed4xINTbK&algo_pvid=85438cd9-87fb-461a-a49e-1895714d06f8&algo_expid=85438cd9-87fb-461a-a49e-1895714d06f8-1&btsid=2c237def-5b7e-4fcf-a843-5a81d01d2e21&ws_ab_test=searchweb0_0,searchweb201602_7,searchweb201603_52 | $100    |
   | Dual FSESC6.6                  | Control the hub motor                    | https://flipsky.net/collections/electronic-products/products/dual-fsesc6-6-based-upon-vesc6-with-aluminum-heatsink | $249    |
   | AERDU 10S3P 10.5Ah 36V Battery | Power the skateboard                     | https://www.aliexpress.com/item/4000275785818.html?spm=a2g0o.productlist.0.0.55137318LRslKf&s=p&algo_pvid=56e535dc-9487-4a74-a745-b38deeadceef&algo_expid=56e535dc-9487-4a74-a745-b38deeadceef-2&btsid=56dde487-691c-4f1a-9e25-ff929ef88092&ws_ab_test=searchweb0_0,searchweb201602_7,searchweb201603_52 | $116.46 |
   | AERDU 10S Battery Charger      | Charge the  battery                      | https://www.aliexpress.com/item/4000275803538.html?gps-id=pcStoreJustForYou&scm=1007.23125.122752.0&scm_id=1007.23125.122752.0&scm-url=1007.23125.122752.0&pvid=5d90e70b-f4bc-4771-a4a8-c11aa5f3a56d&spm=a2g0o.store_home.smartJustForYou_331514713.8 | $12.14  |
   | FlipSky AntiSpark Switch       | On/off and anti spark                    | https://www.hglrc.com/products/hglrc-flipsky-anti-spark-switch-for-electric-longboard-rc-car-e-bike?variant=13801941434410&currency=USD&https://www.hglrc.com/collections/new-arrivals&gclid=CjwKCAiA8ejuBRAaEiwAn-iJ3mSxh7tjnEVt2jdG82gYQyXo5P4AHZkvVNe4WtLBshjYXAiqf2JfQBoCg3AQAvD_BwE | $39     |
   | Battery Percentage Indicator   | Indicate battery percentage              | https://www.mboards.co/products/battery-percentage-indicator | $10     |
   | Skateboard Stand               | For people to stand on                   | https://www.skateshred.com/40-x-9-5-bottlenose-top-mount-blank-deck.html | $35     |
   | WS2812 LED strips 1m           | For board decoration                     | https://www.amazon.com/BTF-LIGHTING-60pixels-Individually-Addressable-Non-waterproof/dp/B07BTTY4FL/ref=sr_1_7?keywords=ws2812%2Bled%2Bstrips%2B1m&qid=1574731675&sr=8-7&th=1 | $18     |
   | Arduino*2                      | For RC control and customizable features | Find at roboclub                                             | $0      |
   | NRF24L01*2                     | For RC Control                           | https://www.amazon.com/Aideepen-Wireless-Transceiver-NRF24L01-Antenna/dp/B01ICU18XC/ref=as_li_ss_tl?ie=UTF8&qid=1533398618&sr=8-8&keywords=NRF24L01&linkCode=sl1&tag=howto045-20&linkId=6a0d99d36f781543f23f967281c11309 | $6      |
   | Other Component                |                                          | Little circuit component like MOSFET and resisters can be find at roboclub | $0      |
   | Total                          |                                          |                                                              | $585.6  |