# sync
```
module Counter_3bit (
  input wire CLK,
  output reg [2:0] Q
);

  always @(posedge CLK) begin
    if (Q == 3'b000)
      Q <= 3'b111;
    else
      Q <= Q - 1;
  end

endmodule

```
![image](https://github.com/sarveshjustin/sync/assets/113497481/9d4b171f-a52d-446b-adc2-beac303977f5)
