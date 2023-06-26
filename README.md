# sync
```
module zen(
  input wire CLK,
  output reg [2:0] Q
);

  reg [2:0] T;

  always @(posedge CLK) begin
    T <= ~Q; 
    Q <= T & Q;
  end

endmodule
```
![image](https://github.com/sarveshjustin/sync/assets/113497481/9d4b171f-a52d-446b-adc2-beac303977f5)
