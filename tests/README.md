<!-- coderabbit-ai-generated:v1 -->

# Single mode simulator

Run `python3 tests/bw16_simulator.py` from the repository root with Python 3 and a C++ compiler (`CXX` can select a different compiler). The tests extract the current Single and AutoSingle functions from the sketch and simulate scan results, buttons, time and radio calls. Two AutoSingle cases are marked as expected failures to make the known stale target and simulated scan channel problems visible; if either starts passing, remove its `expectedFailure` marker.

This simulator does not emulate the BW16 processor, display, radio, or the complete firmware. It does not verify real transmission or device behavior; those require a physical board.