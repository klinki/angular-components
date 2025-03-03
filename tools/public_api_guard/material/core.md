## API Report File for "components-srcs"

> Do not edit this file. It is a report generated by [API Extractor](https://api-extractor.com/).

```ts

import { _AbstractConstructor as _AbstractConstructor_2 } from '@angular/material/core';
import { AbstractControl } from '@angular/forms';
import { AfterViewChecked } from '@angular/core';
import { BooleanInput } from '@angular/cdk/coercion';
import { ChangeDetectorRef } from '@angular/core';
import { _Constructor as _Constructor_2 } from '@angular/material/core';
import { ElementRef } from '@angular/core';
import { EventEmitter } from '@angular/core';
import { FocusableOption } from '@angular/cdk/a11y';
import { FocusOrigin } from '@angular/cdk/a11y';
import { FormGroupDirective } from '@angular/forms';
import { HighContrastModeDetector } from '@angular/cdk/a11y';
import * as i0 from '@angular/core';
import * as i1 from '@angular/cdk/bidi';
import * as i4 from '@angular/common';
import { InjectionToken } from '@angular/core';
import { NgControl } from '@angular/forms';
import { NgForm } from '@angular/forms';
import { NgZone } from '@angular/core';
import { Observable } from 'rxjs';
import { OnDestroy } from '@angular/core';
import { OnInit } from '@angular/core';
import { Platform } from '@angular/cdk/platform';
import { QueryList } from '@angular/core';
import { Subject } from 'rxjs';
import { Version } from '@angular/core';

// @public
export type _AbstractConstructor<T = object> = abstract new (...args: any[]) => T;

// @public
export class AnimationCurves {
    // (undocumented)
    static ACCELERATION_CURVE: string;
    // (undocumented)
    static DECELERATION_CURVE: string;
    // (undocumented)
    static SHARP_CURVE: string;
    // (undocumented)
    static STANDARD_CURVE: string;
}

// @public
export class AnimationDurations {
    // (undocumented)
    static COMPLEX: string;
    // (undocumented)
    static ENTERING: string;
    // (undocumented)
    static EXITING: string;
}

// @public
export interface CanColor {
    color: ThemePalette;
    defaultColor: ThemePalette | undefined;
}

// @public
export interface CanDisable {
    disabled: boolean;
}

// @public
export interface CanDisableRipple {
    disableRipple: boolean;
}

// @public
export interface CanUpdateErrorState {
    errorState: boolean;
    errorStateMatcher: ErrorStateMatcher;
    updateErrorState(): void;
}

// @public
export type _Constructor<T> = new (...args: any[]) => T;

// @public
export function _countGroupLabelsBeforeOption(optionIndex: number, options: QueryList<MatOption>, optionGroups: QueryList<MatOptgroup>): number;

// @public
export abstract class DateAdapter<D, L = any> {
    abstract addCalendarDays(date: D, days: number): D;
    abstract addCalendarMonths(date: D, months: number): D;
    abstract addCalendarYears(date: D, years: number): D;
    clampDate(date: D, min?: D | null, max?: D | null): D;
    abstract clone(date: D): D;
    compareDate(first: D, second: D): number;
    abstract createDate(year: number, month: number, date: number): D;
    deserialize(value: any): D | null;
    abstract format(date: D, displayFormat: any): string;
    abstract getDate(date: D): number;
    abstract getDateNames(): string[];
    abstract getDayOfWeek(date: D): number;
    abstract getDayOfWeekNames(style: 'long' | 'short' | 'narrow'): string[];
    abstract getFirstDayOfWeek(): number;
    abstract getMonth(date: D): number;
    abstract getMonthNames(style: 'long' | 'short' | 'narrow'): string[];
    abstract getNumDaysInMonth(date: D): number;
    getValidDateOrNull(obj: unknown): D | null;
    abstract getYear(date: D): number;
    abstract getYearName(date: D): string;
    abstract invalid(): D;
    abstract isDateInstance(obj: any): boolean;
    abstract isValid(date: D): boolean;
    protected locale: L;
    readonly localeChanges: Observable<void>;
    // (undocumented)
    protected readonly _localeChanges: Subject<void>;
    abstract parse(value: any, parseFormat: any): D | null;
    sameDate(first: D | null, second: D | null): boolean;
    setLocale(locale: L): void;
    abstract today(): D;
    abstract toIso8601(date: D): string;
}

// @public
export const defaultRippleAnimationConfig: {
    enterDuration: number;
    exitDuration: number;
};

// @public
export class ErrorStateMatcher {
    // (undocumented)
    isErrorState(control: AbstractControl | null, form: FormGroupDirective | NgForm | null): boolean;
    // (undocumented)
    static ɵfac: i0.ɵɵFactoryDeclaration<ErrorStateMatcher, never>;
    // (undocumented)
    static ɵprov: i0.ɵɵInjectableDeclaration<ErrorStateMatcher>;
}

// @public
export function _getOptionScrollPosition(optionOffset: number, optionHeight: number, currentScrollPosition: number, panelHeight: number): number;

// @public
export interface GranularSanityChecks {
    // (undocumented)
    doctype: boolean;
    // (undocumented)
    theme: boolean;
    // (undocumented)
    version: boolean;
}

// @public
export interface HasInitialized {
    initialized: Observable<void>;
    _markInitialized: () => void;
}

// @public
export interface HasTabIndex {
    defaultTabIndex: number;
    tabIndex: number;
}

// @public (undocumented)
export const MAT_DATE_FORMATS: InjectionToken<MatDateFormats>;

// @public
export const MAT_DATE_LOCALE: InjectionToken<{}>;

// @public
export function MAT_DATE_LOCALE_FACTORY(): {};

// @public (undocumented)
export const MAT_NATIVE_DATE_FORMATS: MatDateFormats;

// @public
export const MAT_OPTGROUP: InjectionToken<MatOptgroup>;

// @public
export const MAT_OPTION_PARENT_COMPONENT: InjectionToken<MatOptionParentComponent>;

// @public
export const MAT_RIPPLE_GLOBAL_OPTIONS: InjectionToken<RippleGlobalOptions>;

// @public
export class MatCommonModule {
    constructor(highContrastModeDetector: HighContrastModeDetector, _sanityChecks: SanityChecks, _document: Document);
    // (undocumented)
    static ɵfac: i0.ɵɵFactoryDeclaration<MatCommonModule, [null, { optional: true; }, null]>;
    // (undocumented)
    static ɵinj: i0.ɵɵInjectorDeclaration<MatCommonModule>;
    // (undocumented)
    static ɵmod: i0.ɵɵNgModuleDeclaration<MatCommonModule, never, [typeof i1.BidiModule], [typeof i1.BidiModule]>;
}

// @public (undocumented)
export type MatDateFormats = {
    parse: {
        dateInput: any;
    };
    display: {
        dateInput: any;
        monthLabel?: any;
        monthYearLabel: any;
        dateA11yLabel: any;
        monthYearA11yLabel: any;
    };
};

// @public
export const MATERIAL_SANITY_CHECKS: InjectionToken<SanityChecks>;

// @public
export class MatLine {
    // (undocumented)
    static ɵdir: i0.ɵɵDirectiveDeclaration<MatLine, "[mat-line], [matLine]", never, {}, {}, never, never, false, never>;
    // (undocumented)
    static ɵfac: i0.ɵɵFactoryDeclaration<MatLine, never>;
}

// @public (undocumented)
export class MatLineModule {
    // (undocumented)
    static ɵfac: i0.ɵɵFactoryDeclaration<MatLineModule, never>;
    // (undocumented)
    static ɵinj: i0.ɵɵInjectorDeclaration<MatLineModule>;
    // (undocumented)
    static ɵmod: i0.ɵɵNgModuleDeclaration<MatLineModule, [typeof MatLine], [typeof i1_2.MatCommonModule], [typeof MatLine, typeof i1_2.MatCommonModule]>;
}

// @public (undocumented)
export class MatNativeDateModule {
    // (undocumented)
    static ɵfac: i0.ɵɵFactoryDeclaration<MatNativeDateModule, never>;
    // (undocumented)
    static ɵinj: i0.ɵɵInjectorDeclaration<MatNativeDateModule>;
    // (undocumented)
    static ɵmod: i0.ɵɵNgModuleDeclaration<MatNativeDateModule, never, [typeof NativeDateModule], never>;
}

// @public
export class MatOptgroup extends _MatOptgroupBase {
    // (undocumented)
    static ɵcmp: i0.ɵɵComponentDeclaration<MatOptgroup, "mat-optgroup", ["matOptgroup"], { "disabled": "disabled"; }, {}, never, ["*", "mat-option, ng-container"], false, never>;
    // (undocumented)
    static ɵfac: i0.ɵɵFactoryDeclaration<MatOptgroup, never>;
}

// @public (undocumented)
export class _MatOptgroupBase extends _MatOptgroupMixinBase implements CanDisable {
    constructor(parent?: MatOptionParentComponent);
    _inert: boolean;
    label: string;
    _labelId: string;
    // (undocumented)
    static ɵdir: i0.ɵɵDirectiveDeclaration<_MatOptgroupBase, never, never, { "label": "label"; }, {}, never, never, false, never>;
    // (undocumented)
    static ɵfac: i0.ɵɵFactoryDeclaration<_MatOptgroupBase, [{ optional: true; }]>;
}

// @public
export class MatOption<T = any> extends _MatOptionBase<T> {
    constructor(element: ElementRef<HTMLElement>, changeDetectorRef: ChangeDetectorRef, parent: MatOptionParentComponent, group: MatOptgroup);
    // (undocumented)
    static ɵcmp: i0.ɵɵComponentDeclaration<MatOption<any>, "mat-option", ["matOption"], {}, {}, never, ["*"], false, never>;
    // (undocumented)
    static ɵfac: i0.ɵɵFactoryDeclaration<MatOption<any>, [null, null, { optional: true; }, { optional: true; }]>;
}

// @public (undocumented)
export class _MatOptionBase<T = any> implements FocusableOption, AfterViewChecked, OnDestroy {
    constructor(_element: ElementRef<HTMLElement>, _changeDetectorRef: ChangeDetectorRef, _parent: MatOptionParentComponent, group: _MatOptgroupBase);
    get active(): boolean;
    deselect(): void;
    get disabled(): boolean;
    set disabled(value: BooleanInput);
    get disableRipple(): boolean;
    focus(_origin?: FocusOrigin, options?: FocusOptions): void;
    _getAriaSelected(): boolean | null;
    _getHostElement(): HTMLElement;
    getLabel(): string;
    _getTabIndex(): string;
    // (undocumented)
    readonly group: _MatOptgroupBase;
    _handleKeydown(event: KeyboardEvent): void;
    id: string;
    get multiple(): boolean | undefined;
    // (undocumented)
    ngAfterViewChecked(): void;
    // (undocumented)
    ngOnDestroy(): void;
    readonly onSelectionChange: EventEmitter<MatOptionSelectionChange<T>>;
    select(): void;
    get selected(): boolean;
    _selectViaInteraction(): void;
    setActiveStyles(): void;
    setInactiveStyles(): void;
    readonly _stateChanges: Subject<void>;
    value: T;
    get viewValue(): string;
    // (undocumented)
    static ɵdir: i0.ɵɵDirectiveDeclaration<_MatOptionBase<any>, never, never, { "value": "value"; "id": "id"; "disabled": "disabled"; }, { "onSelectionChange": "onSelectionChange"; }, never, never, false, never>;
    // (undocumented)
    static ɵfac: i0.ɵɵFactoryDeclaration<_MatOptionBase<any>, never>;
}

// @public (undocumented)
export class MatOptionModule {
    // (undocumented)
    static ɵfac: i0.ɵɵFactoryDeclaration<MatOptionModule, never>;
    // (undocumented)
    static ɵinj: i0.ɵɵInjectorDeclaration<MatOptionModule>;
    // (undocumented)
    static ɵmod: i0.ɵɵNgModuleDeclaration<MatOptionModule, [typeof i1_3.MatOption, typeof i2.MatOptgroup], [typeof i3.MatRippleModule, typeof i4.CommonModule, typeof i1_2.MatCommonModule, typeof i6.MatPseudoCheckboxModule], [typeof i1_3.MatOption, typeof i2.MatOptgroup]>;
}

// @public
export interface MatOptionParentComponent {
    // (undocumented)
    disableRipple?: boolean;
    // (undocumented)
    inertGroups?: boolean;
    // (undocumented)
    multiple?: boolean;
}

// @public
export class MatOptionSelectionChange<T = any> {
    constructor(
    source: _MatOptionBase<T>,
    isUserInput?: boolean);
    isUserInput: boolean;
    source: _MatOptionBase<T>;
}

// @public
export class MatPseudoCheckbox {
    constructor(_animationMode?: string | undefined);
    // (undocumented)
    _animationMode?: string | undefined;
    disabled: boolean;
    state: MatPseudoCheckboxState;
    // (undocumented)
    static ɵcmp: i0.ɵɵComponentDeclaration<MatPseudoCheckbox, "mat-pseudo-checkbox", never, { "state": "state"; "disabled": "disabled"; }, {}, never, never, false, never>;
    // (undocumented)
    static ɵfac: i0.ɵɵFactoryDeclaration<MatPseudoCheckbox, [{ optional: true; }]>;
}

// @public (undocumented)
export class MatPseudoCheckboxModule {
    // (undocumented)
    static ɵfac: i0.ɵɵFactoryDeclaration<MatPseudoCheckboxModule, never>;
    // (undocumented)
    static ɵinj: i0.ɵɵInjectorDeclaration<MatPseudoCheckboxModule>;
    // (undocumented)
    static ɵmod: i0.ɵɵNgModuleDeclaration<MatPseudoCheckboxModule, [typeof i1_5.MatPseudoCheckbox], [typeof i1_2.MatCommonModule], [typeof i1_5.MatPseudoCheckbox]>;
}

// @public
export type MatPseudoCheckboxState = 'unchecked' | 'checked' | 'indeterminate';

// @public (undocumented)
export class MatRipple implements OnInit, OnDestroy, RippleTarget {
    constructor(_elementRef: ElementRef<HTMLElement>, ngZone: NgZone, platform: Platform, globalOptions?: RippleGlobalOptions, _animationMode?: string | undefined);
    animation: RippleAnimationConfig;
    centered: boolean;
    color: string;
    get disabled(): boolean;
    set disabled(value: boolean);
    fadeOutAll(): void;
    fadeOutAllNonPersistent(): void;
    launch(config: RippleConfig): RippleRef;
    launch(x: number, y: number, config?: RippleConfig): RippleRef;
    // (undocumented)
    ngOnDestroy(): void;
    // (undocumented)
    ngOnInit(): void;
    radius: number;
    get rippleConfig(): RippleConfig;
    get rippleDisabled(): boolean;
    get trigger(): HTMLElement;
    set trigger(trigger: HTMLElement);
    unbounded: boolean;
    // (undocumented)
    static ɵdir: i0.ɵɵDirectiveDeclaration<MatRipple, "[mat-ripple], [matRipple]", ["matRipple"], { "color": "matRippleColor"; "unbounded": "matRippleUnbounded"; "centered": "matRippleCentered"; "radius": "matRippleRadius"; "animation": "matRippleAnimation"; "disabled": "matRippleDisabled"; "trigger": "matRippleTrigger"; }, {}, never, never, false, never>;
    // (undocumented)
    static ɵfac: i0.ɵɵFactoryDeclaration<MatRipple, [null, null, null, { optional: true; }, { optional: true; }]>;
}

// @public (undocumented)
export class MatRippleModule {
    // (undocumented)
    static ɵfac: i0.ɵɵFactoryDeclaration<MatRippleModule, never>;
    // (undocumented)
    static ɵinj: i0.ɵɵInjectorDeclaration<MatRippleModule>;
    // (undocumented)
    static ɵmod: i0.ɵɵNgModuleDeclaration<MatRippleModule, [typeof i1_4.MatRipple], [typeof i1_2.MatCommonModule], [typeof i1_4.MatRipple, typeof i1_2.MatCommonModule]>;
}

// @public
export function mixinColor<T extends _AbstractConstructor<HasElementRef>>(base: T, defaultColor?: ThemePalette): CanColorCtor & T;

// @public
export function mixinDisabled<T extends _AbstractConstructor<{}>>(base: T): CanDisableCtor & T;

// @public
export function mixinDisableRipple<T extends _AbstractConstructor<{}>>(base: T): CanDisableRippleCtor & T;

// @public
export function mixinErrorState<T extends _AbstractConstructor<HasErrorState>>(base: T): CanUpdateErrorStateCtor & T;

// @public
export function mixinInitialized<T extends _Constructor<{}>>(base: T): HasInitializedCtor & T;

// @public
export function mixinTabIndex<T extends _AbstractConstructor<CanDisable>>(base: T, defaultTabIndex?: number): HasTabIndexCtor & T;

// @public
export class NativeDateAdapter extends DateAdapter<Date> {
    constructor(matDateLocale: string,
    _platform?: Platform);
    // (undocumented)
    addCalendarDays(date: Date, days: number): Date;
    // (undocumented)
    addCalendarMonths(date: Date, months: number): Date;
    // (undocumented)
    addCalendarYears(date: Date, years: number): Date;
    // (undocumented)
    clone(date: Date): Date;
    // (undocumented)
    createDate(year: number, month: number, date: number): Date;
    deserialize(value: any): Date | null;
    // (undocumented)
    format(date: Date, displayFormat: Object): string;
    // (undocumented)
    getDate(date: Date): number;
    // (undocumented)
    getDateNames(): string[];
    // (undocumented)
    getDayOfWeek(date: Date): number;
    // (undocumented)
    getDayOfWeekNames(style: 'long' | 'short' | 'narrow'): string[];
    // (undocumented)
    getFirstDayOfWeek(): number;
    // (undocumented)
    getMonth(date: Date): number;
    // (undocumented)
    getMonthNames(style: 'long' | 'short' | 'narrow'): string[];
    // (undocumented)
    getNumDaysInMonth(date: Date): number;
    // (undocumented)
    getYear(date: Date): number;
    // (undocumented)
    getYearName(date: Date): string;
    // (undocumented)
    invalid(): Date;
    // (undocumented)
    isDateInstance(obj: any): boolean;
    // (undocumented)
    isValid(date: Date): boolean;
    // (undocumented)
    parse(value: any, parseFormat?: any): Date | null;
    // (undocumented)
    today(): Date;
    // (undocumented)
    toIso8601(date: Date): string;
    // @deprecated (undocumented)
    useUtcForDisplay: boolean;
    // (undocumented)
    static ɵfac: i0.ɵɵFactoryDeclaration<NativeDateAdapter, [{ optional: true; }, null]>;
    // (undocumented)
    static ɵprov: i0.ɵɵInjectableDeclaration<NativeDateAdapter>;
}

// @public (undocumented)
export class NativeDateModule {
    // (undocumented)
    static ɵfac: i0.ɵɵFactoryDeclaration<NativeDateModule, never>;
    // (undocumented)
    static ɵinj: i0.ɵɵInjectorDeclaration<NativeDateModule>;
    // (undocumented)
    static ɵmod: i0.ɵɵNgModuleDeclaration<NativeDateModule, never, never, never>;
}

// @public
export interface RippleAnimationConfig {
    enterDuration?: number;
    exitDuration?: number;
}

// @public (undocumented)
export type RippleConfig = {
    color?: string;
    centered?: boolean;
    radius?: number;
    persistent?: boolean;
    animation?: RippleAnimationConfig;
    terminateOnPointerUp?: boolean;
};

// @public
export interface RippleGlobalOptions {
    animation?: RippleAnimationConfig;
    disabled?: boolean;
    terminateOnPointerUp?: boolean;
}

// @public
export class RippleRef {
    constructor(_renderer: {
        fadeOutRipple(ref: RippleRef): void;
    },
    element: HTMLElement,
    config: RippleConfig, _animationForciblyDisabledThroughCss?: boolean);
    // (undocumented)
    _animationForciblyDisabledThroughCss: boolean;
    config: RippleConfig;
    element: HTMLElement;
    fadeOut(): void;
    state: RippleState;
}

// @public
export class RippleRenderer implements EventListenerObject {
    constructor(_target: RippleTarget, _ngZone: NgZone, elementOrElementRef: HTMLElement | ElementRef<HTMLElement>, platform: Platform);
    fadeInRipple(x: number, y: number, config?: RippleConfig): RippleRef;
    fadeOutAll(): void;
    fadeOutAllNonPersistent(): void;
    fadeOutRipple(rippleRef: RippleRef): void;
    handleEvent(event: Event): void;
    _removeTriggerEvents(): void;
    setupTriggerEvents(elementOrElementRef: HTMLElement | ElementRef<HTMLElement>): void;
}

// @public
export const enum RippleState {
    // (undocumented)
    FADING_IN = 0,
    // (undocumented)
    FADING_OUT = 2,
    // (undocumented)
    HIDDEN = 3,
    // (undocumented)
    VISIBLE = 1
}

// @public
export interface RippleTarget {
    rippleConfig: RippleConfig;
    rippleDisabled: boolean;
}

// @public
export type SanityChecks = boolean | GranularSanityChecks;

// @public
export function setLines(lines: QueryList<unknown>, element: ElementRef<HTMLElement>, prefix?: string): void;

// @public
export class ShowOnDirtyErrorStateMatcher implements ErrorStateMatcher {
    // (undocumented)
    isErrorState(control: AbstractControl | null, form: FormGroupDirective | NgForm | null): boolean;
    // (undocumented)
    static ɵfac: i0.ɵɵFactoryDeclaration<ShowOnDirtyErrorStateMatcher, never>;
    // (undocumented)
    static ɵprov: i0.ɵɵInjectableDeclaration<ShowOnDirtyErrorStateMatcher>;
}

// @public
export type ThemePalette = 'primary' | 'accent' | 'warn' | undefined;

// @public
export const VERSION: Version;

// (No @packageDocumentation comment for this package)

```
