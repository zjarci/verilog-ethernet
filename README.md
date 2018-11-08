# Verilog Ethernet Components Readme

For more information and updates: http://alexforencich.com/wiki/en/verilog/ethernet/start

GitHub repository: https://github.com/alexforencich/verilog-ethernet

## Introduction

Collection of Ethernet-related components for both gigabit and 10G packet
processing (8 bit and 64 bit datapaths).  Includes modules for handling
Ethernet frames as well as IP, UDP, and ARP and the components for
constructing a complete UDP/IP stack.  Includes full MyHDL testbench with
intelligent bus cosimulation endpoints.

For IP and ARP support only, use ip_complete (1G) or ip_complete_64 (10G).

For UDP, IP, and ARP support, use udp_complete (1G) or udp_complete_64 (10G).

## Documentation

### arp module

ARP handling logic with parametrizable retry timeout parameters.

### arp_64 module

ARP handling logic with parametrizable retry timeout parameters and 64 bit
datapath for 10G Ethernet.

### arp_cache module

Basic hash-based cache for ARP entries.  Parametrizable depth.  

### arp_eth_rx module

ARP frame receiver.

### arp_eth_rx_64 module

ARP frame receiver with 64 bit datapath for 10G Ethernet.

### arp_eth_tx module

ARP frame transmitter.

### arp_eth_tx_64 module

ARP frame transmitter with 64 bit datapath for 10G Ethernet.

### axis_eth_fcs module

Ethernet frame check sequence calculator.

### axis_eth_fcs_64 module

Ethernet frame check sequence calculator with 64 bit datapath for 10G Ethernet.

### axis_eth_fcs_check module

Ethernet frame check sequence checker.

### axis_eth_fcs_insert module

Ethernet frame check sequence inserter.

### axis_gmii_rx module

AXI stream GMII/MII frame receiver with clock enable and MII select.

### axis_gmii_tx module

AXI stream GMII/MII frame transmitter with clock enable and MII select.

### axis_xgmii_rx_32 module

AXI stream XGMII frame receiver with 32 bit datapath.

### axis_xgmii_rx_64 module

AXI stream XGMII frame receiver with 64 bit datapath.

### axis_xgmii_tx_32 module

AXI stream XGMII frame transmitter with 32 bit datapath.

### axis_xgmii_tx_64 module

AXI stream XGMII frame transmitter with 64 bit datapath.

### eth_arb_mux module

Ethernet frame arbitrated muliplexer with parametrizable data width and port
count.  Supports priority and round-robin arbitration.

### eth_axis_rx module

Ethernet frame receiver.

### eth_axis_rx_64 module

Ethernet frame receiver with 64 bit datapath for 10G Ethernet.

### eth_axis_tx module

Ethernet frame transmitter.

### eth_axis_tx_64 module

Ethernet frame transmitter with 64 bit datapath for 10G Ethernet.

### eth_demux module

Ethernet frame demuliplexer with parametrizable data width and port count.
Supports priority and round-robin arbitration.

### eth_mac_1g module

Gigabit Ethernet MAC with GMII interface.

### eth_mac_1g_fifo module

Gigabit Ethernet MAC with GMII interface and FIFOs.

### eth_mac_1g_gmii module

Tri-mode Ethernet MAC with GMII/MII interface and automatic PHY rate
adaptation logic.

### eth_mac_1g_gmii_fifo module

Tri-mode Ethernet MAC with GMII/MII interface, FIFOs, and automatic PHY rate
adaptation logic.

### eth_mac_1g_rgmii module

Tri-mode Ethernet MAC with RGMII interface and automatic PHY rate adaptation
logic.

### eth_mac_1g_rgmii_fifo module

Tri-mode Ethernet MAC with RGMII interface, FIFOs, and automatic PHY rate
adaptation logic.

### eth_mac_10g module

10G Ethernet MAC with XGMII interface.  Datapath selectable between 32 and 64
bits.

### eth_mac_10g_fifo module

10G Ethernet MAC with XGMII interface and FIFOs.  Datapath selectable between
32 and 64 bits.

### eth_mux module

Ethernet frame muliplexer with parametrizable data width and port count.
Supports priority and round-robin arbitration.

### gmii_phy_if

GMII/MII PHY interface and clocking logic.

### ip module

IPv4 block with 8 bit data width for gigabit Ethernet.  Manages IPv4 packet
transmssion and reception.  Interfaces with ARP module for MAC address lookup.

### ip_64 module

IPv4 block with 64 bit data width for 10G Ethernet.  Manages IPv4 packet
transmssion and reception.  Interfaces with ARP module for MAC address lookup.

### ip_arb_mux module

IP frame arbitrated muliplexer with parametrizable data width and port count.
Supports priority and round-robin arbitration.

### ip_complete module

IPv4 module with ARP integration.

Top level for gigabit IP stack.

### ip_complete_64 module

IPv4 module with ARP integration and 64 bit data width for 10G Ethernet.

Top level for 10G IP stack.

### ip_demux module

IP frame demuliplexer with parametrizable data width and port count.
Supports priority and round-robin arbitration.

### ip_eth_rx module

IP frame receiver.

### ip_eth_rx_64 module

IP frame receiver with 64 bit datapath for 10G Ethernet.

### ip_eth_tx module

IP frame transmitter.

### ip_eth_tx_64 module

IP frame transmitter with 64 bit datapath for 10G Ethernet.

### ip_mux module

IP frame muliplexer with parametrizable data width and port count.
Supports priority and round-robin arbitration.

### lfsr module

Fully parametrizable combinatorial parallel LFSR/CRC module.

### rgmii_phy_if

RGMII PHY interface and clocking logic.

### udp module

UDP block with 8 bit data width for gigabit Ethernet.  Manages UDP packet
transmssion and reception.

### udp_64 module

UDP block with 64 bit data width for 10G Ethernet.  Manages UDP packet
transmssion and reception.

### udp_arb_mux module

UDP frame arbitrated muliplexer with parametrizable data width and port
count.  Supports priority and round-robin arbitration.

### udp_checksum_gen module

UDP checksum generator module.  Calculates UDP length, IP length, and
UDP checksum fields.

### udp_checksum_gen_64 module

UDP checksum generator module with 64 bit datapath.  Calculates UDP
length, IP length, and UDP checksum fields.

### udp_complete module

UDP module with IPv4 and ARP integration.

Top level for gigabit UDP stack.

### udp_complete_64 module

UDP module with IPv4 and ARP integration and 64 bit data width for 10G
Ethernet.

Top level for 10G UDP stack.

### udp_demux module

UDP frame demuliplexer with parametrizable data width and port count.
Supports priority and round-robin arbitration.

### udp_ip_rx module

UDP frame receiver.

### udp_ip_rx_64 module

UDP frame receiver with 64 bit datapath for 10G Ethernet.

### udp_ip_tx module

UDP frame transmitter.

### udp_ip_tx_64 module

UDP frame transmitter with 64 bit datapath for 10G Ethernet.

### udp_mux module

UDP frame muliplexer with parametrizable data width and port count.
Supports priority and round-robin arbitration.

### xgmii_deinterleave.v

XGMII de-interleaver for interfacing with PHY cores that interleave the
control and data lines.

### xgmii_interleave.v

XGMII interleaver for interfacing with PHY cores that interleave the control
and data lines.

### Common signals

    tdata   : Data (width generally DATA_WIDTH)
    tkeep   : Data word valid (width generally KEEP_WIDTH, present on _64 modules)
    tvalid  : Data valid
    tready  : Sink ready
    tlast   : End-of-frame
    tuser   : Bad frame (valid with tlast & tvalid)

### Source Files

    rtl/arp.v                       : ARP handling logic
    rtl/arp_64.v                    : ARP handling logic (64 bit)
    rtl/arp_cache.v                 : ARP LRU cache
    rtl/arp_eth_rx.v                : ARP frame receiver
    rtl/arp_eth_rx_64.v             : ARP frame receiver (64 bit)
    rtl/arp_eth_tx.v                : ARP frame transmitter
    rtl/arp_eth_tx_64.v             : ARP frame transmitter (64 bit)
    rtl/eth_arb_mux.py              : Ethernet frame arbitrated multiplexer generator
    rtl/axis_eth_fcs.v              : Ethernet FCS calculator
    rtl/axis_eth_fcs_64.v           : Ethernet FCS calculator (64 bit)
    rtl/axis_eth_fcs_insert.v       : Ethernet FCS inserter
    rtl/axis_eth_fcs_check.v        : Ethernet FCS checker
    rtl/axis_gmii_rx.v              : AXI stream GMII/MII receiver
    rtl/axis_gmii_tx.v              : AXI stream GMII/MII transmitter
    rtl/axis_xgmii_rx_32.v          : AXI stream XGMII receiver (32 bit)
    rtl/axis_xgmii_rx_64.v          : AXI stream XGMII receiver (64 bit)
    rtl/axis_xgmii_tx_32.v          : AXI stream XGMII transmitter (32 bit)
    rtl/axis_xgmii_tx_64.v          : AXI stream XGMII transmitter (64 bit)
    rtl/eth_arb_mux.v               : Ethernet frame arbitrated multiplexer
    rtl/eth_axis_rx.v               : Ethernet frame receiver
    rtl/eth_axis_rx_64.v            : Ethernet frame receiver (64 bit)
    rtl/eth_axis_tx.v               : Ethernet frame transmitter
    rtl/eth_axis_tx_64.v            : Ethernet frame transmitter (64 bit)
    rtl/eth_demux.v                 : Ethernet frame demultiplexer
    rtl/eth_mac_1g.v                : Gigabit Etherent GMII MAC
    rtl/eth_mac_1g_fifo.v           : Gigabit Etherent GMII MAC with FIFO
    rtl/eth_mac_1g_gmii.v           : Tri-mode Ethernet GMII/MII MAC
    rtl/eth_mac_1g_gmii_fifo.v      : Tri-mode Ethernet GMII/MII MAC with FIFO
    rtl/eth_mac_1g_rgmii.v          : Tri-mode Ethernet RGMII MAC
    rtl/eth_mac_1g_rgmii_fifo.v     : Tri-mode Ethernet RGMII MAC with FIFO
    rtl/eth_mac_10g.v               : 10G Etherent XGMII MAC
    rtl/eth_mac_10g_fifo.v          : 10G Etherent XGMII MAC with FIFO
    rtl/eth_mux.v                   : Ethernet frame multiplexer
    rtl/gmii_phy_if.v               : GMII PHY interface
    rtl/iddr.v                      : Generic DDR input register
    rtl/ip.v                        : IPv4 block
    rtl/ip_64.v                     : IPv4 block (64 bit)
    rtl/ip_arb_mux.v                : IP frame arbitrated multiplexer
    rtl/ip_complete.v               : IPv4 stack (IP-ARP integration)
    rtl/ip_complete_64.v            : IPv4 stack (IP-ARP integration) (64 bit)
    rtl/ip_demux.v                  : IP frame demultiplexer
    rtl/ip_eth_rx.v                 : IPv4 frame receiver
    rtl/ip_eth_rx_64.v              : IPv4 frame receiver (64 bit)
    rtl/ip_eth_tx.v                 : IPv4 frame transmitter
    rtl/ip_eth_tx_64.v              : IPv4 frame transmitter (64 bit)
    rtl/ip_mux.v                    : IP frame multiplexer
    rtl/lfsr.v                      : Generic LFSR/CRC module
    rtl/oddr.v                      : Generic DDR output register
    rtl/rgmii_phy_if.v              : RGMII PHY interface
    rtl/ssio_ddr_in.v               : Generic source synchronous IO DDR input module
    rtl/ssio_ddr_in_diff.v          : Generic source synchronous IO DDR differential input module
    rtl/ssio_ddr_out.v              : Generic source synchronous IO DDR output module
    rtl/ssio_ddr_out_diff.v         : Generic source synchronous IO DDR differential output module
    rtl/ssio_sdr_in.v               : Generic source synchronous IO SDR input module
    rtl/ssio_sdr_in_diff.v          : Generic source synchronous IO SDR differential input module
    rtl/ssio_sdr_out.v              : Generic source synchronous IO SDR output module
    rtl/ssio_sdr_out_diff.v         : Generic source synchronous IO SDR differential output module
    rtl/udp.v                       : UDP block
    rtl/udp_64.v                    : UDP block (64 bit)
    rtl/udp_arb_mux.v               : UDP frame arbitrated multiplexer
    rtl/udp_checksum_gen.v          : UDP checksum generator
    rtl/udp_checksum_gen_64.v       : UDP checksum generator (64 bit)
    rtl/udp_complete.v              : UDP stack (IP-ARP-UDP)
    rtl/udp_complete_64.v           : UDP stack (IP-ARP-UDP) (64 bit)
    rtl/udp_demux.v                 : UDP frame demultiplexer
    rtl/udp_ip_rx.v                 : UDP frame receiver
    rtl/udp_ip_rx_64.v              : UDP frame receiver (64 bit)
    rtl/udp_ip_tx.v                 : UDP frame transmitter
    rtl/udp_ip_tx_64.v              : UDP frame transmitter (64 bit)
    rtl/udp_mux.v                   : UDP frame multiplexer

### AXI Stream Interface Example

transfer with header data

                  __    __    __    __    __    __    __
    clk        __/  \__/  \__/  \__/  \__/  \__/  \__/  \__
               ______________                   ___________
    hdr_ready                \_________________/
                        _____ 
    hdr_valid  ________/     \_____________________________
                        _____
    hdr_data   XXXXXXXXX_HDR_XXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
                        ___________ _____ _____
    tdata      XXXXXXXXX_A0________X_A1__X_A2__XXXXXXXXXXXX
                        ___________ _____ _____
    tkeep      XXXXXXXXX_K0________X_K1__X_K2__XXXXXXXXXXXX
                        _______________________
    tvalid     ________/                       \___________
                              _________________
    tready     ______________/                 \___________
                                          _____
    tlast      __________________________/     \___________

    tuser      ____________________________________________


two byte transfer with sink pause after each byte

              __    __    __    __    __    __    __    __    __
    clk    __/  \__/  \__/  \__/  \__/  \__/  \__/  \__/  \__/  \__
                    _____ _________________
    tdata  XXXXXXXXX_D0__X_D1______________XXXXXXXXXXXXXXXXXXXXXXXX
                    _____ _________________
    tkeep  XXXXXXXXX_K0__X_K1______________XXXXXXXXXXXXXXXXXXXXXXXX
                    _______________________
    tvalid ________/                       \_______________________
           ______________             _____             ___________
    tready               \___________/     \___________/
                          _________________
    tlast  ______________/                 \_______________________

    tuser  ________________________________________________________


two back-to-back packets, no pauses

              __    __    __    __    __    __    __    __    __
    clk    __/  \__/  \__/  \__/  \__/  \__/  \__/  \__/  \__/  \__
                    _____ _____ _____ _____ _____ _____
    tdata  XXXXXXXXX_A0__X_A1__X_A2__X_B0__X_B1__X_B2__XXXXXXXXXXXX
                    _____ _____ _____ _____ _____ _____
    tkeep  XXXXXXXXX_K0__X_K1__X_K2__X_K0__X_K1__X_K2__XXXXXXXXXXXX
                    ___________________________________
    tvalid ________/                                   \___________
           ________________________________________________________
    tready
                                _____             _____
    tlast  ____________________/     \___________/     \___________

    tuser  ________________________________________________________


bad frame

              __    __    __    __    __    __
    clk    __/  \__/  \__/  \__/  \__/  \__/  \__
                    _____ _____ _____
    tdata  XXXXXXXXX_A0__X_A1__X_A2__XXXXXXXXXXXX
                    _____ _____ _____
    tkeep  XXXXXXXXX_K0__X_K1__X_K2__XXXXXXXXXXXX
                    _________________
    tvalid ________/                 \___________
           ______________________________________
    tready
                                _____
    tlast  ____________________/     \___________
                                _____
    tuser  ____________________/     \___________


## Testing

Running the included testbenches requires MyHDL and Icarus Verilog.  Make sure
that myhdl.vpi is installed properly for cosimulation to work correctly.  The
testbenches can be run with a Python test runner like nose or py.test, or the
individual test scripts can be run with python directly.

### Testbench Files

    tb/arp_ep.py         : MyHDL ARP frame endpoints
    tb/axis_ep.py        : MyHDL AXI Stream endpoints
    tb/eth_ep.py         : MyHDL Ethernet frame endpoints
    tb/gmii_ep.py        : MyHDL GMII endpoints
    tb/ip_ep.py          : MyHDL IP frame endpoints
    tb/rgmii_ep.py       : MyHDL RGMII endpoints
    tb/udp_ep.py         : MyHDL UDP frame endpoints
    tb/xgmii_ep.py       : MyHDL XGMII endpoints
