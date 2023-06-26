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
