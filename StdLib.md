## String
- .append(data: string): void
- .prepend(data: string): void
- .appendCharCode(data: u32): void
- .prependCharCode(data: u32): void
- .insert(data: string, position: u32): void
- .insertCharCode(data: u32, position: u32): void
- .at(index: u32): string
- .charAt(index: u32): string
- .charCodeAt(index: u32): u32
- .includes(search: string): boolean
- .startsWith(search: string): boolean
- .endsWith(search: string): boolean
- .replace(search: string, replacement: string): string
- .replaceAll(search: string, replacement: string): string
- .findIndex(search: string): u32
- .findLastIndex(search: string): u32
- .split(seperator: string): Array\<string>
- .trim(): string
- .trimLeft(): string
- .trimRight(): string
## Number
- .toString(): string
- .NaN: boolean
- *static* .isFinite(): boolean
- *static* .isInfinite(): boolean
- *static* .isFloat(): boolean
- *static* .isInteger(): boolean
- *static* .isSigned(): boolean
- *static* .isNaN(): boolean
## Boolean
- .toString(): string
## Function
- *static* .name: string
- *static* .toString(): string
- *static* .index: u32
## Object
- *static* .keys(o: Object): Array<string>
- *static* .values(o: Object): Array<any>
- .freeze(o: Object): Object
- .set(key: string, value: any): void
- .get(key: string): any
- .toString(): any
## Array
- .append(data: T): void
- .prepend(data: T): void
- .at(index: u32): T
- .shift(): T
- .pop(): T
- .has(search): boolean
- .findIndex(search): u32
- .reverse(): Array\<T>
- .length: u32
- .slice(start: u32, end: u32): Array\<T>
- .join(seperator: string | null = null): string
## JSON
- .stringify(data: any): string
- .parse(data: string): any
- .isValid(data: string): boolean
## Console
- .log(data: any): void
## Math
- .abs\<T>(num: T): T
- .acos\<T>(num: T): T
- .acosh\<T>(num: T): T
- .asin\<T>(num: T): T
- .asinh\<T>(num: T): T
- .atan\<T>(num: T): T
- .atan2\<T>(y: T, x: T): T
- .atanh\<T>(num: T): T
- .cbrt\<T>(num: T): T
- .ceil\<T>(num: T): T
- .clz32\<T>(num: T): T
- .cos\<T>(num: T): T
- .cosh\<T>(num: T): T
- .exp\<T>(num: T): T
- .floor\<T>(num: T): T
- .fround\<T>(num: T): T
- .hypot\<T>(num: ...T[]): T
- .imul\<T>(x: T, y): T
- .log\<T>(num: T): T
- .log10\<T>(num: T): T
- .log1p\<T>(num: T): T
- .log2\<T>(num: T): T
- .max\<T>(num: ...T[]): T
- .min\<T>(num: ...T[]): T
- .pow\<T>(x: T, y: T): T
- .random\<T>(): f64 (0.0-1.0)
- .randomInt\<T>(): u32 (0-9)
- .sin\<T>(num: T): T
- .sinh\<T>(num: T): T
- .sqrt\<T>(num: T): T
- .tan\<T>(num: T): T
- .tanh\<T>(num: T): T
- .trunc\<T>(num: T): T
## Time
- *static* .now(): u64
- *static* .hours(): u32
- *static* .minutes(): u32
- *static* .seconds(): u32
- *static* .nanoseconds(): u32
## FileSystem
- .writeFile\<T>(path: string, data: T): void
- .readFile(path: string): Buffer
- .appendFile\<T>(path: string, data: T): void
- .prependFile\<T>(path: string, data: T): void
## Buffer
- *static* .from\<T>(data: T): Buffer
- .toString(encoding: string | null): string
## Stream
- .write(data: T): void
- .pipe(stream: Stream): void
- .on(event: string, callback: () => {})
- .close()
- .pause()
- .resume()
## process
- .exit(code: u32 | null): void
- .nextTick?
