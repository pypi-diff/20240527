# Comparing `tmp/systrack-0.5.tar.gz` & `tmp/systrack-0.5rc1.tar.gz`

## Comparing `systrack-0.5.tar` & `systrack-0.5rc1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     5629 2020-02-02 00:00:00.000000 systrack-0.5/CHANGELOG.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 systrack-0.5/src/systrack/__init__.py
--rw-r--r--   0        0        0    11424 2020-02-02 00:00:00.000000 systrack-0.5/src/systrack/__main__.py
--rw-r--r--   0        0        0     5371 2020-02-02 00:00:00.000000 systrack-0.5/src/systrack/elf.py
--rw-r--r--   0        0        0     3730 2020-02-02 00:00:00.000000 systrack-0.5/src/systrack/kconfig.py
--rw-r--r--   0        0        0    27501 2020-02-02 00:00:00.000000 systrack-0.5/src/systrack/kconfig_options.py
--rw-r--r--   0        0        0    23472 2020-02-02 00:00:00.000000 systrack-0.5/src/systrack/kernel.py
--rw-r--r--   0        0        0    15932 2020-02-02 00:00:00.000000 systrack-0.5/src/systrack/location.py
--rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 systrack-0.5/src/systrack/output.py
--rw-r--r--   0        0        0     6467 2020-02-02 00:00:00.000000 systrack-0.5/src/systrack/signature.py
--rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 systrack-0.5/src/systrack/syscall.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 systrack-0.5/src/systrack/type_hints.py
--rw-r--r--   0        0        0     9508 2020-02-02 00:00:00.000000 systrack-0.5/src/systrack/utils.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 systrack-0.5/src/systrack/version.py
--rw-r--r--   0        0        0     5496 2020-02-02 00:00:00.000000 systrack-0.5/src/systrack/arch/__init__.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 systrack-0.5/src/systrack/arch/all.py
--rw-r--r--   0        0        0    11829 2020-02-02 00:00:00.000000 systrack-0.5/src/systrack/arch/arch_base.py
--rw-r--r--   0        0        0     5664 2020-02-02 00:00:00.000000 systrack-0.5/src/systrack/arch/arm.py
--rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 systrack-0.5/src/systrack/arch/arm64.py
--rw-r--r--   0        0        0     4139 2020-02-02 00:00:00.000000 systrack-0.5/src/systrack/arch/mips.py
--rw-r--r--   0        0        0    13498 2020-02-02 00:00:00.000000 systrack-0.5/src/systrack/arch/powerpc.py
--rw-r--r--   0        0        0    22558 2020-02-02 00:00:00.000000 systrack-0.5/src/systrack/arch/x86.py
--rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 systrack-0.5/src/systrack/templates/syscall_table.css
--rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 systrack-0.5/src/systrack/templates/syscall_table.html
--rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 systrack-0.5/src/systrack/templates/syscall_table.js
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 systrack-0.5/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 systrack-0.5/LICENSE
--rw-r--r--   0        0        0     5747 2020-02-02 00:00:00.000000 systrack-0.5/README.md
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 systrack-0.5/pyproject.toml
--rw-r--r--   0        0        0     7132 2020-02-02 00:00:00.000000 systrack-0.5/PKG-INFO
+-rw-r--r--   0        0        0     4371 2020-02-02 00:00:00.000000 systrack-0.5rc1/CHANGELOG.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 systrack-0.5rc1/src/systrack/__init__.py
+-rw-r--r--   0        0        0    11424 2020-02-02 00:00:00.000000 systrack-0.5rc1/src/systrack/__main__.py
+-rw-r--r--   0        0        0     5371 2020-02-02 00:00:00.000000 systrack-0.5rc1/src/systrack/elf.py
+-rw-r--r--   0        0        0     3730 2020-02-02 00:00:00.000000 systrack-0.5rc1/src/systrack/kconfig.py
+-rw-r--r--   0        0        0    27501 2020-02-02 00:00:00.000000 systrack-0.5rc1/src/systrack/kconfig_options.py
+-rw-r--r--   0        0        0    23039 2020-02-02 00:00:00.000000 systrack-0.5rc1/src/systrack/kernel.py
+-rw-r--r--   0        0        0    15907 2020-02-02 00:00:00.000000 systrack-0.5rc1/src/systrack/location.py
+-rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 systrack-0.5rc1/src/systrack/output.py
+-rw-r--r--   0        0        0     6467 2020-02-02 00:00:00.000000 systrack-0.5rc1/src/systrack/signature.py
+-rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 systrack-0.5rc1/src/systrack/syscall.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 systrack-0.5rc1/src/systrack/type_hints.py
+-rw-r--r--   0        0        0     9508 2020-02-02 00:00:00.000000 systrack-0.5rc1/src/systrack/utils.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 systrack-0.5rc1/src/systrack/version.py
+-rw-r--r--   0        0        0     5496 2020-02-02 00:00:00.000000 systrack-0.5rc1/src/systrack/arch/__init__.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 systrack-0.5rc1/src/systrack/arch/all.py
+-rw-r--r--   0        0        0    11829 2020-02-02 00:00:00.000000 systrack-0.5rc1/src/systrack/arch/arch_base.py
+-rw-r--r--   0        0        0     5664 2020-02-02 00:00:00.000000 systrack-0.5rc1/src/systrack/arch/arm.py
+-rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 systrack-0.5rc1/src/systrack/arch/arm64.py
+-rw-r--r--   0        0        0     4139 2020-02-02 00:00:00.000000 systrack-0.5rc1/src/systrack/arch/mips.py
+-rw-r--r--   0        0        0    13498 2020-02-02 00:00:00.000000 systrack-0.5rc1/src/systrack/arch/powerpc.py
+-rw-r--r--   0        0        0    22639 2020-02-02 00:00:00.000000 systrack-0.5rc1/src/systrack/arch/x86.py
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 systrack-0.5rc1/src/systrack/templates/syscall_table.css
+-rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 systrack-0.5rc1/src/systrack/templates/syscall_table.html
+-rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 systrack-0.5rc1/src/systrack/templates/syscall_table.js
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 systrack-0.5rc1/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 systrack-0.5rc1/LICENSE
+-rw-r--r--   0        0        0     5747 2020-02-02 00:00:00.000000 systrack-0.5rc1/README.md
+-rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 systrack-0.5rc1/pyproject.toml
+-rw-r--r--   0        0        0     7139 2020-02-02 00:00:00.000000 systrack-0.5rc1/PKG-INFO
```

### Comparing `systrack-0.5/CHANGELOG.md` & `systrack-0.5rc1/CHANGELOG.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,41 +1,10 @@
 Systrack changelog
 ==================
 
-v0.5
-----
-
-We tried so hard, and got so far, but in the end, we need a disassembler! x86
-mitigations have defeated us, we no longer have syscall tables to rely on.
-Kernel developers were kind enough to write very simple ABI-specific
-switch-based handlers to dispach syscalls, so analysis is still possible... just
-significantly more complicated.
-
-**Breaking changes**:
-
-- Drop support for Python 3.6 and 3.7. Systrack now requires Python 3.8+. This
-  is because of the new dependency on
-  [`iced-x86`](https://pypi.org/project/iced-x86/).
-
-**Improvements**:
-
-- x86: support new kernels (6.9+) with no syscall tables.
-- Remove unnecessary spaces between asterisks for double pointers in function
-  signatures.
-- Avoid KFCI `__{cfi,pfx}_` symbols when looking for `ni_syscall` symbols.
-
-**Internal changes**:
-
-- Depend on [`iced-x86`](https://pypi.org/project/iced-x86/) for disassembling
-  x86 instructions and on [`jinja2`](https://pypi.org/project/jinja2/) for HTML
-  output directly. Remove optional dependencies and only build one package.
-- Rename `test` folder to `tests` to use the `hatch test` as test commnad
-- Improve logging reproducibility by sorting more debugging log output.
-- Improve broken Python package metadata (Python packaging moment).
-
 v0.4
 ----
 
 New arch support: PowerPC 32-bit, tested on v5.0+ kernels.
 
 **Improvements**:
```

### Comparing `systrack-0.5/src/systrack/__main__.py` & `systrack-0.5rc1/src/systrack/__main__.py`

 * *Files identical despite different names*

### Comparing `systrack-0.5/src/systrack/elf.py` & `systrack-0.5rc1/src/systrack/elf.py`

 * *Files identical despite different names*

### Comparing `systrack-0.5/src/systrack/kconfig.py` & `systrack-0.5rc1/src/systrack/kconfig.py`

 * *Files identical despite different names*

### Comparing `systrack-0.5/src/systrack/kconfig_options.py` & `systrack-0.5rc1/src/systrack/kconfig_options.py`

 * *Files identical despite different names*

### Comparing `systrack-0.5/src/systrack/kernel.py` & `systrack-0.5rc1/src/systrack/kernel.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import struct
 import atexit
 from pathlib import Path
 from time import monotonic
 from os import sched_getaffinity
 from operator import itemgetter, attrgetter
 from collections import defaultdict, Counter
-from typing import Tuple, List, Dict, Iterator, Union, Any, Optional
+from typing import Tuple, List, Dict, Iterator, Union, Any
 
 from .arch import arch_from_name, arch_from_vmlinux
 from .elf import ELF, Symbol, Section
 from .kconfig import edit_config, edit_config_check_deps
 from .kconfig import kconfig_more_syscalls, kconfig_debugging
 from .kconfig import kconfig_compatibility, kconfig_syscall_deps
 from .location import extract_syscall_locations
@@ -37,18 +37,17 @@
 	__version         = None
 	__version_source  = None
 	__syscalls        = None
 	__backup_makefile = None
 	__long_size       = None
 	__long_pack_fmt   = None
 
-	def __init__(self, arch_name: Optional[str] = None,
-			vmlinux: Optional[Path] = None, kdir: Optional[Path] = None,
-			outdir: Optional[Path] = None, rdir: Optional[Path] = None,
-			toolchain_prefix: Optional[str] = None):
+	def __init__(self, arch_name: str = None, vmlinux: Path = None,
+			kdir: Path = None, outdir: Path = None, rdir: Path = None,
+			toolchain_prefix: str = None):
 		if not kdir and not vmlinux:
 			raise ValueError('at least one of vmlinux or kdir is needed')
 		if arch_name is None and vmlinux is None:
 			raise ValueError('need vmlinux to determine arch if not supplied')
 
 		self.kdir             = kdir
 		self.outdir           = outdir
@@ -334,17 +333,16 @@
 
 		seen = set(vaddrs.values())
 		symbols_by_vaddr = {sym.vaddr: sym for sym in ni_syscalls}
 		discarded_logs = []
 		preferred_logs = []
 
 		# Create a mapping vaddr -> symbol for every vaddr in the syscall table
-		# for convenience. Sort symbols by name for reproducible results. We
-		# look at .symbols instead of .functions here because (of course) some
-		# of these symbols may not be classified as FUNC.
+		# for convenience. Sort symbols by name to generate reproducible results
+		# and logs.
 		for sym in sorted(self.vmlinux.symbols.values(), key=attrgetter('name')):
 			vaddr = sym.vaddr
 			if vaddr not in seen:
 				continue
 
 			other = symbols_by_vaddr.get(vaddr)
 			if sym == other:
@@ -361,19 +359,14 @@
 				sym, other = pref, (other if pref is sym else sym)
 
 				if high_verbosity():
 					preferred_logs.append((pref.name, other.name))
 
 			symbols_by_vaddr[vaddr] = sym
 
-		# Sort logs for reproducible output (the above sorting does not
-		# guarantee that these are sorted as well).
-		discarded_logs.sort()
-		preferred_logs.sort()
-
 		for sym, other in discarded_logs:
 			logging.debug('Discarding %s as alias for %s', sym, other)
 
 		for sym, other in preferred_logs:
 			logging.debug('Preferring %s over %s', sym, other)
 
 		del discarded_logs
@@ -437,18 +430,15 @@
 
 			symbols.append((idx, sym))
 			symbol_names.append(sym.name)
 
 		# Find common syscall symbol prefixes (e.g. "__x64_sys_") in order to be
 		# able to strip them later to obtain the actual syscall name
 		prefixes = common_syscall_symbol_prefixes(symbol_names, 20)
-		if prefixes:
-			logging.info('Common syscall symbol prefixes: %s', ', '.join(prefixes))
-		else:
-			logging.warn('No common syscall symbol prefixes found (weird!)')
+		logging.info('Common syscall symbol prefixes: %s', ', '.join(prefixes))
 
 		syscalls  = []
 		n_skipped = 0
 
 		# Build list of syscalls (with prefixes stripped from the names) and
 		# skip uneeded ones (e.g. implemented for other ABIs)
 		for idx, sym in symbols:
@@ -508,15 +498,15 @@
 		# Nonetheless, do a first pass to filter out syscalls with dummy
 		# implementation and avoid unnecessary source code grepping to find
 		# their definitions.
 		syscalls = list(filter(lambda s: not self.arch.is_dummy_syscall(s, self.vmlinux), syscalls))
 
 		# Find locations and signatures for all the syscalls we found (except
 		# esoteric ones).
-		extract_syscall_locations(syscalls, self.vmlinux, self.arch, self.kdir, self.rdir)
+		extract_syscall_locations(syscalls, self.vmlinux, self.kdir, self.rdir, self.arch)
 		extract_syscall_signatures(syscalls, self.vmlinux, self.kdir is not None)
 
 		# Second pass to extract only implemented syscalls: warn for potentially
 		# bad matches and filter out invalid ones.
 		implemented  = []
 		bad_loc_info = []
 		no_loc_info  = []
```

### Comparing `systrack-0.5/src/systrack/location.py` & `systrack-0.5rc1/src/systrack/location.py`

 * *Files 1% similar despite different names*

```diff
@@ -214,16 +214,15 @@
 			# Found start of function body (weird)
 			logging.debug('Found start of function body, but not the actual '
 				'signature: %s:%d', file, i + 1)
 			return i + 1
 
 	return line
 
-def extract_syscall_locations(syscalls: List[Syscall], vmlinux: ELF, arch: Arch,
-		kdir: Optional[Path], rdir: Optional[Path]):
+def extract_syscall_locations(syscalls: List[Syscall], vmlinux: ELF, kdir: Path, rdir: Path, arch: Arch):
 	if not command_available('addr2line'):
 		logging.warning('Command "addr2line" unavailable, skipping location info extraction')
 		return
 
 	# STEP 1: Ask addr2line for file/lineno info. Most of the times this will
 	# work with at most a simple line adjustment.
 
@@ -236,15 +235,15 @@
 			sc.file = file
 			sc.line = line
 			sc.good_location = False
 
 		if any(map(attrgetter('file'), syscalls)):
 			logging.warning('No kernel source available, trusting addr2line output for location info')
 		else:
-			logging.warning('No kernel source available and no addr2line output, cannot extract location info')
+			logging.info('No kernel source available and no addr2line output, cannot extract location info')
 
 		return
 
 	rel = lambda p: maybe_rel(p, kdir)
 	bad_paths = False
 	to_adjust = []
 	to_retry = []
```

### Comparing `systrack-0.5/src/systrack/output.py` & `systrack-0.5rc1/src/systrack/output.py`

 * *Files identical despite different names*

### Comparing `systrack-0.5/src/systrack/signature.py` & `systrack-0.5rc1/src/systrack/signature.py`

 * *Files identical despite different names*

### Comparing `systrack-0.5/src/systrack/syscall.py` & `systrack-0.5rc1/src/systrack/syscall.py`

 * *Files identical despite different names*

### Comparing `systrack-0.5/src/systrack/utils.py` & `systrack-0.5rc1/src/systrack/utils.py`

 * *Files identical despite different names*

### Comparing `systrack-0.5/src/systrack/arch/__init__.py` & `systrack-0.5rc1/src/systrack/arch/__init__.py`

 * *Files identical despite different names*

### Comparing `systrack-0.5/src/systrack/arch/arch_base.py` & `systrack-0.5rc1/src/systrack/arch/arch_base.py`

 * *Files identical despite different names*

### Comparing `systrack-0.5/src/systrack/arch/arm.py` & `systrack-0.5rc1/src/systrack/arch/arm.py`

 * *Files identical despite different names*

### Comparing `systrack-0.5/src/systrack/arch/arm64.py` & `systrack-0.5rc1/src/systrack/arch/arm64.py`

 * *Files identical despite different names*

### Comparing `systrack-0.5/src/systrack/arch/mips.py` & `systrack-0.5rc1/src/systrack/arch/mips.py`

 * *Files identical despite different names*

### Comparing `systrack-0.5/src/systrack/arch/powerpc.py` & `systrack-0.5rc1/src/systrack/arch/powerpc.py`

 * *Files identical despite different names*

### Comparing `systrack-0.5/src/systrack/arch/x86.py` & `systrack-0.5rc1/src/systrack/arch/x86.py`

 * *Files 1% similar despite different names*

```diff
@@ -334,15 +334,15 @@
 		if code[:3] == b'\x48\xc7\xc0' and code[3:7] in bad_imm: # mov rax, -ENOSYS/-EINVAL
 			if sz == 8  and code[7] == 0xc3: return orig # ret
 			if sz == 9  and code[7] == 0xeb: return orig # jmp rel8
 			if sz == 12 and code[7] == 0xe9: return orig # jmp rel32
 
 		return None
 
-	def __emulate_syscall_switch(self, func: Symbol, func_code: bytes) -> Optional[Tuple[DefaultDict[int,Set[int]],Set[Instruction]]]:
+	def __emulate_syscall_switch(self, func: Symbol, func_code: bytes) -> Optional[Tuple[DefaultDict[int,Set[int]],Set[Instruction],DefaultDict[Instruction,int]]]:
 		start = func.real_vaddr
 		end   = func.real_vaddr + func.size
 		insns = list(Decoder(32 if self.bits32 else 64, func_code, ip=start))
 
 		# Register used to hold syscall number
 		nr_reg = None
 
@@ -365,15 +365,15 @@
 		jccs = {JA, JAE, JB, JBE, JE, JNE}
 		# Maximum syscall number supported plus 1
 		nr_max = 0x1000
 		# Possible syscall numbers at a given address (instruction pointer)
 		nrs: DefaultDict[int,Set[int]] = defaultdict(set, {start: set(range(nr_max))})
 		# Candidate branches to syscall functions
 		candidate_insns: Set[Instruction] = set()
-		# Accumulate non-NOP skipped insns for logging/debugging purposes
+		# Accumulate non-NOP skipped insns for debugging purposes
 		skipped_insns: DefaultDict[Instruction,int] = defaultdict(int)
 
 		keep_going = True
 		iteration = 0
 
 		# Symbolically trace the function code to determine the possible syscall
 		# numbers and the instructions that lead to them
@@ -488,39 +488,32 @@
 					nrs[next_ip] |= cur_nrs
 					continue
 
 				# We get here for JMP, Jcc and CALL near
 				if start <= target_ip < end:
 					# Branch target inside function
 					if target_ip < ip:
-						# Backward branch: new numbers may be added to the
+						# Backward branch, new numbers may be added to the
 						# target instruction, but we are already past it. In
 						# such case, we'll need an additional iteration to
 						# propagate the information.
 						if not new_taken_nrs.issubset(nrs[target_ip]):
 							keep_going = True
 				else:
-					# Branch target outside function, assume it's a branch to a
+					# Branch target outsize function, assume it's a branch to a
 					# syscall function
 					candidate_insns.add(insn)
 
 				nrs[target_ip] |= new_taken_nrs
 				nrs[next_ip] |= new_not_taken_nrs
 
 		logging.info('Symbolic emulation done in %d iteration%s', iteration,
 			's'[:iteration ^ 1])
 
-		if skipped_insns:
-			n_skipped = sum(skipped_insns.values())
-			skipped = sorted(skipped_insns.items(), key=itemgetter(1, 0), reverse=True)
-			skipped = '; '.join((f'{i:r} (x{n})' for i, n in skipped))
-			logging.debug('Skipped %d instruction%s: %s', n_skipped,
-				's'[:n_skipped ^ 1], skipped)
-
-		return nrs, candidate_insns
+		return nrs, candidate_insns, skipped_insns
 
 	def extract_syscall_vaddrs(self, vmlinux: ELF) -> Dict[int,int]:
 		# We need to go through a painful examination of the switch statement
 		# implemented by {x64,x32,ia32}_sys_call():
 		#
 		#    #define __SYSCALL(nr, sym) case nr: return __x64_##sym(regs);
 		#
@@ -544,38 +537,47 @@
 			logging.error('Could not find function %s', func_name)
 			return {}
 
 		if sym.size < 0x10:
 			logging.error('%s is too small (%d bytes)', sym.name, sym.size)
 			return {}
 
-		logging.info('Extracting syscalls from code of %s() at %#x', sym.name,
+		logging.info('Recovering syscalls from code of %s() at %#x', sym.name,
 			sym.real_vaddr)
 
 		res = self.__emulate_syscall_switch(sym, vmlinux.read_symbol(sym))
 		if res is None:
 			return {}
 
-		nrs, candidate_insns = res
+		nrs, candidate_insns, skipped_insns = res
+
+		if skipped_insns:
+			n_skipped = sum(skipped_insns.values())
+			skipped = sorted(skipped_insns.items(), key=itemgetter(1, 0), reverse=True)
+			skipped = '; '.join((f'{i:r} (x{n})' for i, n in skipped))
+			logging.debug('Skipped %d instruction%s: %s', n_skipped,
+				's'[:n_skipped ^ 1], skipped)
+
 		vaddrs: Dict[int,int] = {}
 		found_default_case = False
 
 		for insn in candidate_insns:
 			# Guaranteed to have .near_branch_target by the code in
 			# __emulate_syscall_switch() above
 			vaddr = insn.near_branch_target
 			numbers = nrs[vaddr]
 
 			if len(numbers) == 0:
 				# This should never happen, bail out
-				logging.error('Empty set of syscall numbers for %#x (target of '
-					'%r). Unreachable!?', vaddr, insn)
+				logging.error('Empty set of syscall numbers for %#x. '
+					'Unreachable???', vaddr)
 				return {}
 
 			if len(numbers) > 100:
+				# This is definitely the default switch case
 				logging.debug('Default switch case at %#x (reachable %d '
 					'times): %r => %#x is ni_syscall', insn.ip,
 					len(numbers), insn, vaddr)
 
 				if found_default_case:
 					logging.error('Multiple default switch cases?')
 					return {}
```

### Comparing `systrack-0.5/src/systrack/templates/syscall_table.css` & `systrack-0.5rc1/src/systrack/templates/syscall_table.css`

 * *Files identical despite different names*

### Comparing `systrack-0.5/src/systrack/templates/syscall_table.html` & `systrack-0.5rc1/src/systrack/templates/syscall_table.html`

 * *Files identical despite different names*

### Comparing `systrack-0.5/src/systrack/templates/syscall_table.js` & `systrack-0.5rc1/src/systrack/templates/syscall_table.js`

 * *Files identical despite different names*

### Comparing `systrack-0.5/LICENSE` & `systrack-0.5rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `systrack-0.5/README.md` & `systrack-0.5rc1/README.md`

 * *Files identical despite different names*

### Comparing `systrack-0.5/pyproject.toml` & `systrack-0.5rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 	'iced-x86~=1.21.0',
 	'jinja2~=3.1.2'
 ]
 
 [project.urls]
 Homepage = 'https://github.com/mebeim/systrack'
 Repository = 'https://github.com/mebeim/systrack.git'
-Changelog = 'https://github.com/mebeim/systrack/blob/master/CHANGELOG.md'
+Changelog = 'https://github.com/mebeim/systrack.git/blob/master/CHANGELOG.md'
 
 [project.scripts]
 systrack = 'systrack.__main__:main'
 
 [build-system]
 requires = ['hatchling']
 build-backend = 'hatchling.build'
```

### Comparing `systrack-0.5/PKG-INFO` & `systrack-0.5rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.3
 Name: systrack
-Version: 0.5
+Version: 0.5rc1
 Summary: Linux kernel syscall implementation tracker
 Project-URL: Homepage, https://github.com/mebeim/systrack
 Project-URL: Repository, https://github.com/mebeim/systrack.git
-Project-URL: Changelog, https://github.com/mebeim/systrack/blob/master/CHANGELOG.md
+Project-URL: Changelog, https://github.com/mebeim/systrack.git/blob/master/CHANGELOG.md
 Author: Marco Bonelli
 Author-email: Marco Bonelli <marco@mebeim.net>
 Maintainer: Marco Bonelli
 Maintainer-email: Marco Bonelli <marco@mebeim.net>
 License: GNU General Public License v3 (GPLv3)
 License-File: LICENSE
 Keywords: abi,elf,kconfig,kernel,linux,syscall,systrack
```

