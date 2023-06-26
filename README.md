# grey
```
module grey(
  input [3:0] gray,
  output reg [3:0] binary
);

  always @(*)
  begin
    binary[3] = gray[3];
    binary[2] = binary[3] ^ gray[2];
    binary[1] = binary[2] ^ gray[1];
    binary[0] = binary[1] ^ gray[0];
  end

endmodule
```
![image](https://github.com/sarveshjustin/grey/assets/113497481/248bbb15-70d0-429e-9cdc-d4f3e2eadac6)

