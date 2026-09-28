# Under-Voltage-protection-system
# Under Voltage Protection System
# Python Simulation Program

print("======================================")
print("       UNDER VOLTAGE PROTECTION")
print("======================================")

# Safe voltage limit
MIN_VOLTAGE = 200
NORMAL_VOLTAGE = 230

# Get input voltage
voltage = float(input("Enter input voltage (V): "))

print("\n----------- SYSTEM STATUS -----------")
print("Input Voltage :", voltage, "V")
print("Minimum Safe Voltage :", MIN_VOLTAGE, "V")

# Protection logic
if voltage < MIN_VOLTAGE:
    print("\n⚠️ UNDER VOLTAGE DETECTED!")
    print("🔴 Protection System Activated")
    print("🔌 Load Disconnected")

elif voltage < NORMAL_VOLTAGE:
    print("\n🟡 Voltage is LOW but within the safe limit")
    print("🟢 Load remains connected")

else:
    print("\n🟢 Voltage is NORMAL")
    print("✅ Load remains connected")

print("\n======================================")
print("       MONITORING COMPLETED")
print("======================================")
