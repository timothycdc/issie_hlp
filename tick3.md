# Tick3 Readme
1. Setup
2. `npm run dev`
3. Create new empty Issie project
4. Developer Mode
5. Run Tick3 tests within window top toolbar
6. Work out what the tests do
7. Write a test of Issie's automatic wire routing
8. Trace start of Test 1
9. Study code in `TestDrawBlock.fs` and `GenerateData.fs`
10. Modify test so that routing is tested between two components at positions as before but with arbitary rotation and component flip
11. Look at `BusWireroute.smartAutoroute` (trace from `placeWire` function). Work out how routing is done, modify it to reduce errors.

## Tests
1. Test 1 
    ```
    Test Horizontally positioned AND + DFF: fail on sample 0 has FAILED on sample 0 with error message:
    Fail (Failing forced on Sample 0.)
     >>Cmd:964 MenuAction (MenuDrawBlockTest ((testIndex, dispatch_1, model) => {: 12.3ms
     >>Cmd:964 UpdateModel (a_1 => new Model(a_1.UserData, a_1.WaveSim, a_1.WaveSimSh: 0.2ms
     findChange: 0.1ms
     >>Cmd:964 Sheet message: 0.4ms
     Sample 0
     >>Cmd:965 UpdateDrawBlockTestState (_arg => {
    const matchValue = result.Test: 0.4ms
     >>Cmd:965 Sheet message: 0.1ms
     findChange: 0.1ms
     >>Cmd:965 Sheet message: 0.3ms
     >>Cmd:965 Sheet message: 0.2ms
     >>Cmd:965 Sheet message: 0.1ms
     >>Cmd:966 Sheet message: 0.2ms
     >>>View: 1.2ms
    ```
  **Sample Data:**

    
